# Interpreting Hungarian
## English ↔ Hungarian translation skill for AI agents

`"Ha már Mesterséges Intelligenciát használsz magyar szöveg készítésére, legalább tedd úgy, mint akinek van esze. (Mondod te a modellnek, melyet alkalmazol)"`

Ez a SKILL Fable 5-el készült, összesen 15M token van mögötte, és még mindig jobb, ha te is belematatsz az AI generált szövegbe, de ezzel valószínűleg jobb eredményt érsz el mint nélküle. Még akár Fable 5 és GPT 5.6 esettében is. Sonnet 5, Opus 4.8, GLM 5.2, Kimi 2.7 és DeepSeek V4 simán megbírja és ezekkel a modellekkel is lehet közel végleges MI szöveget készíteni a SKILL alkalmazásával.

Translate English to Hungarian and Hungarian to English the way a native writes, not the way a dictionary maps words. A drop-in [Agent Skill](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) for Claude, Claude Code, Codex, and any agent that reads the Agent Skills format.

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)
![Claude Skill](https://img.shields.io/badge/Claude-Agent%20Skill-7C3AED)
![Language pair](https://img.shields.io/badge/EN%20%E2%87%84%20HU-translation-success)
![Models](https://img.shields.io/badge/Sonnet%205%20%7C%20Opus%204.8%20%7C%20GPT--5.5-tuned-informational)

Hungarian is hard in both directions. A model's raw output usually *parses* — Hungarian translation studies calls the residue *kvázi-helyesség*: every sentence grammatical, the whole still unmistakably translated. Going the other way it produces **Hunglish**: English words in Hungarian word order, the tense system flattened, the articles missing. This skill encodes what closes both gaps — including the devices corpus research shows translations systematically lack, because the source language never prompts them.

## What it catches

Traps a strong model walks into unaided — the middle column is the instinctive translation, and it is wrong:

**English → Hungarian**

| English | Instinctive but wrong | Native |
|---------|----------------------|--------|
| I've lived here for two years. | Két éve itt laktam. *(= two years ago)* | **Két éve itt lakom.** |
| I'm hot. | Meleg vagyok. *(= I'm gay)* | **Melegem van.** |
| You must not smoke here. | Itt nem kell dohányozni. *(= no need to)* | **Itt nem szabad dohányozni.** |
| Do you play tennis? | Játszol teniszt? | **Teniszezel?** |
| I like your dress. | Szeretem a ruhádat. | **Tetszik a ruhád.** |
| I can't help laughing. | Nem tudok segíteni nevetve. | **Muszáj nevetnem.** |
| Mistakes were made. | Hibák lettek elkövetve. | **Hibákat követtek el.** |
| "Come in," said Peter. | "Gyere be," mondta Péter. | **– Gyere be – mondta Péter.** |
| a $5 billion deal | 5 billió dolláros üzlet *(1000× off)* | **5 milliárd dolláros üzlet** |

**Hungarian → English**

| Hungarian | Instinctive but wrong | Native |
|-----------|----------------------|--------|
| Két éve láttam. | I've seen him for two years. | **I saw him two years ago.** |
| Már két éve itt lakom. | I live here since two years. | **I've lived here for two years.** |
| Anna alszik, Péter pedig olvas. | Anna is sleeping, Peter however is reading. | **Anna is sleeping, while Peter is reading.** |
| PÉTER ette meg az almát. | Peter ate the apple. *(emphasis lost)* | **It was Peter who ate the apple.** |
| Senki nem segít. | Nobody doesn't help. | **Nobody helps.** |
| Öten voltunk. | We were five. | **There were five of us.** |
| Azt hiszem, hogy jó. | I think, that it is good. | **I think it's good.** |
| Nagy Éva felhívott. | Nagy Éva called me. | **Éva Nagy called me.** |
| ötmilliárd forint | five milliard forints | **five billion forints** |

Beyond the traps, the skill covers the full system: topic–focus word order, definite vs. indefinite conjugation, coverb aspect, case suffixes, register (te/ön) and its English compensation, relative pronouns, false friends both ways, literary norms (dialogue dashes, no tense backshift, names, titles, form-faithful verse), domain conventions (software UI, Netflix-style subtitles, marketing, plain-language official prose), and punctuation/date/number conventions in both directions. It works as a **diagnostic, not a checklist** — it names over-correction as a failure mode, so already-natural sentences are left alone. And it restores what translated Hungarian statistically lacks (*szokott*, *-lak/-lek*, *hadd*, particles, diminutives): the source text never prompts them, natives use them anyway.

## Install

Core skill in one line (self-contained for everyday English→Hungarian):

```bash
curl -fsSL https://raw.githubusercontent.com/forint573/interpreting-hungarian/main/interpreting-hungarian/SKILL.md --create-dirs -o ~/.claude/skills/interpreting-hungarian/SKILL.md
```

Full folder — recommended, and required for Hungarian→English, literary, and domain work:

```bash
git clone https://github.com/forint573/interpreting-hungarian.git
cp -r interpreting-hungarian/interpreting-hungarian ~/.claude/skills/
```

- **Per project:** use `.claude/skills/` inside the repo instead of `~/.claude/skills/`.
- **Codex / Cursor / Gemini CLI:** copy the same folder into that tool's skills directory (e.g. `~/.codex/skills/`); for agents without skills support, paste `SKILL.md` into the system prompt or `AGENTS.md`.
- **Claude desktop & web apps:** zip the `interpreting-hungarian` folder and upload it under Settings → Capabilities → Skills.
- **Claude API / Agent SDK:** load the folder as an Agent Skill, or drop `SKILL.md` into the system prompt.

## Use

Restart your session and just ask — the skill triggers on anything that looks like English↔Hungarian translation:

- `Translate this email to Hungarian: …`
- `Fordítsd le angolra: …`
- `Localize this landing page for a Hungarian audience.`

It returns only the translation, preserves structure and formatting, leaves code, URLs, brands, and placeholders untouched, and keeps one register per text (domain defaults; formal *ön* when ambiguous — say `informal (te)` or `formal (ön)` to override). Going into English, the dead te/ön distinction is compensated with address forms, directness, and contractions.

## Model notes

- **Claude Sonnet 5 / Claude Opus 4.8** — rules state their scope explicitly, reference files are routed with literal "read before drafting" triggers, and deliberation is directed only where it pays (register maps, names, terminology for long or literary passages). API: default `effort: high` suits everyday texts; `xhigh` pays off for poetry and full-document localization. Sonnet 5 takes no `temperature` — the skill's explicit conventions supply that consistency.
- **GPT-5.5** — written to match its literal instruction-following: absolutes are true invariants (never the *kerül*-passive, only the translation in the reply), everything else is a decision rule judged by outcome. A calibration section in `SKILL.md` addresses each model family by name. Reasoning `medium` is enough for everyday texts, `high` for literary.
- **Other models** run it unchanged — positive patterns first, calque examples as labeled contrast, worked examples throughout.

## Inside the folder

| File | What it holds |
|------|---------------|
| `SKILL.md` | The diagnostic core: EN→HU rules, the HU→EN essentials, routing, output contract, self-checks |
| `reference/hungarian-to-english.md` | Full HU→EN system: reassembly method, tense fan-out, articles, negation, names, register compensation, Hunglish sweep |
| `reference/literary-translation.md` | The műfordítás norms: dialogue dashes, tense discipline, names/titles/realia, verse, transfer operations |
| `reference/domain-conventions.md` | Software UI, subtitles (Netflix limits), marketing, plain-language official prose |
| `reference/grammar-tables.md` | Full paradigms: conjugations, cases, postpositions, possession, vowel harmony |
| `reference/style-lexicon.md` | Greetings, punctuation, dates/numbers, extended false friends, MT tell list |

The core file works alone; the agent pulls reference files in only when the text type needs them, so the always-loaded footprint stays small.

## FAQ

**How do I translate English to Hungarian with Claude Code?** Install the skill, then ask for the translation in plain language — it loads automatically, no flags or API keys.

**Does it translate Hungarian to English too?** Yes — install the full folder; `reference/hungarian-to-english.md` carries that direction.

**Which models and tools?** Tuned for Claude Sonnet 5, Claude Opus 4.8, and GPT-5.5; compatible with earlier models. Works in Claude Code, the Claude apps, Codex, Cursor, the Gemini CLI, and via the API.

**Does it affect other languages?** No — it only activates for English↔Hungarian requests. Free under Apache 2.0.

## Grounding

The rules are drawn from reference grammars (Rounds; É. Kiss on information structure), the Hungarian orthographic standard (AkH. 12.), Klaudy Kinga's transfer-operation framework and translator-training methodology, corpus research on translation universals (the unique-items findings for Hungarian), the műfordítás canon from Arany to Nádasdy, and the professional style guides of the Hungarian localization industry (Microsoft, FSF.hu, Netflix, the EU institutions).

## License

[Apache License 2.0](LICENSE) · Copyright 2026 Virág Làzár Csaba ✸☽

## Keywords

English to Hungarian translation, Hungarian to English translation, translate English to Hungarian, translate Hungarian to English, AI Hungarian translation, idiomatic Hungarian, native Hungarian translation, interpreting Hungarian, Hungarian interpreter AI, magyar fordítás, angol-magyar fordító, angol magyar fordító, angol magyar fordito, magyar-angol fordító, magyar angol fordító, magyar fordító, magyar fordito, műfordítás, Hungarian literary translation, Hungarian subtitles, Hungarian localization, Hungarian UI localization, Hunglish, leiterjakab, Claude skill, Claude Code skill, Claude Agent Skill, Codex skill, Claude Sonnet 5, Claude Opus 4.8, GPT-5.5, machine translation Hungarian, English Hungarian translator, Hungarian English translator.
