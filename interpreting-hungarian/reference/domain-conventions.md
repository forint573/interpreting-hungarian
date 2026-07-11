# Domain conventions: UI, subtitles, marketing, official prose (reference)

Read this file **before drafting** when the source text is software/UI copy, an error message, subtitles or captions, marketing/advertising copy, or official-administrative-legal prose. Each domain has hard conventions that override general prose habits — register above all. The norms below follow the professional style guides used in the Hungarian localization industry (Microsoft Hungarian Style Guide, the FSF.hu/Ubuntu translation HOWTOs, the Netflix Hungarian Timed Text Style Guide, the EU institutions' Hungarian style guide, and Budapest's plain-language handbook).

## 1. Register by domain — the decision table

| Domain | Address | Notes |
|---|---|---|
| Software UI, apps, documentation | **impersonal first, ön second — never te** | Exceptions: products for children; AI-assistant prompt templates (tegező imperatives: *Sorolj fel ötleteket…*) |
| Error messages, system text | impersonal (*A fájl nem található.*) | No blame, no jokes, no "Hoppá" |
| Consumer marketing, e-commerce, social | **te** by default | magázás for conservative, B2B, financial, healthcare, or older audiences; never mix within a campaign |
| Official, government, legal | **Ön** (capitalized in letters) | plain-language rules in §5 |
| Business email | ön (te only if the parties tegeződnek) | salutations: `style-lexicon.md` |
| Subtitles, fiction dialogue | per the on-screen/on-page relationship | decide each character pair once; a te↔ön switch is a plot event |

Consistency beats the choice itself: pronouns, verb forms, possessives, and imperatives must all match one register within a text.

## 2. Software and UI strings

**Buttons, menu items, and command labels are nouns in -ás/-és, not imperatives:**
- Save → **Mentés** · Open → **Megnyitás** · Exit → **Kilépés** · Edit → **Szerkesztés** · View → **Nézet** · Help → **Súgó** · Settings → **Beállítások**
- The two canonical exceptions are verb forms by convention: Apply → **Alkalmaz**, Cancel → **Mégse**.
- Headings and help titles follow the same nominal pattern: *Opening a document / How to open a document* → **Dokumentum megnyitása**.

**Running UI text addresses the user impersonally or with ön (3rd person):**
- Would you like to continue? → **Folytatja?** · Enter the file name. → **Adja meg a fájl nevét.**
- Prefer no pronoun at all; drop English possessives: *your computer* → **a számítógép** (not *az ön számítógépe*).
- Progress text: *Trying to connect…* → **Csatlakozás kezdeményezése…** · *File is being saved* → **A fájl mentése folyamatban van…**

**Error messages** — fixed native patterns, never passive:
- cannot be opened / could not find → **nem nyitható meg / nem található** (the *-ható/-hető* predicative is the idiom)
- failed to… → **nem sikerült…** · is not available → **nem érhető el / nem áll rendelkezésre**
- *The file was created last week.* → **A fájlt a múlt héten hozták létre.** (never *lett létrehozva*)

**Mechanics:**
- Sentence-style capitalization everywhere; English Title Case is an error in Hungarian (*Help and Support* → **Súgó és támogatás**). When citing UI elements, copy the UI's own capitalization: *kattintson a **Tovább** gombra*.
- Imperative sentences end in a **period, not an exclamation mark** (*Adja meg a fájl nevét.*); reserve **!** for genuine warnings (*…az adatai elvesznek!*).
- Placeholders: position the variable so Hungarian syntax survives; use **a(z)** before an unknowable value, or recast (*A következőt nem lehet megnyitni: {name}*). Never inflect a file name or path (*az /etc/lilo.conf fájlt*, not *…lilo.conf-ot*) — attach the suffix to a category noun instead.
- Product names decline with the normal hyphen/assimilation rules: **Wordöt, Office-t, Skype-ban**.
- Gender-neutral by default: *kolléga* not *kolléganő*, plurals for generalization; accessibility phrasing *fogyatékossággal élő személy*.
- Non-breaking space between number and unit (**15 GB**) and in grouped thousands (**100 000**).
- Words the industry style guides ban as officialese: *kíván* (→ **szeretne**), *megkísérel* (→ **megpróbál**), *amennyiben* (→ **ha**), *kerül* periphrases (→ active verb).
- **Two documentation traditions coexist** — match the platform's existing one. Microsoft-style: ön-imperatives (*Kattintson a Tovább gombra.*). Open-source/wiki tradition (FSF.hu, Ubuntu, Wikipedia help): 1st-person plural (*Kattintsunk a Tovább gombra.* · *Nyissuk meg a fájlt.*). Never mix them in one document.
- No causative where the user acts directly: *mentjük a fájlt*, not *mentetjük*; and for data loss prefer **elvész** (*a nem mentett adat elvész*) — *elveszik* misreads as "someone takes it away".

## 3. Subtitles (Netflix timed-text norms)

Hard limits:
- **42 characters per line, max 2 lines** per subtitle; keep to one line when it fits.
- Reading speed: **17 characters/second** for adult programs, **13 cps** for children's.
- Two speakers in one subtitle: **dash + space, one speaker per line**, dash on both lines:
  **- Várj!**
  **- Megvannak az iratok?**

Conventions:
- Condense, don't clip: drop fillers and repetitions first (subtitling is compression — keep speech-act and register, sacrifice redundancy). Do not translate a phrase the same speaker repeats back-to-back.
- **Italics** for: titles of works, foreign words, voice-over narration, dialogue from electronic media / off-scene speakers, and song lyrics. Never italics for emphasis.
- **Numbers:** spell out one through ten (except dates), numerals above ten; spell out any number starting a sentence; decimal comma; five-digit-and-longer numbers grouped with a space; times as 10.00 or 10:00, consistently.
- **Quotes:** „…” with »…« inside.
- **Song lyrics:** each line starts with a capital; line-end punctuation only `?` and `!` (no commas or periods).
- **Ellipsis:** the single … character (U+2026); use it for a pause or interruption, and (without a space) when picking up mid-sentence: **…megszerezte.** No ellipsis when a sentence merely continues into the next subtitle.
- **Forced narratives (on-screen text):** translate only if plot-pertinent, ALL CAPS (long prologue/epilogue passages: sentence case), never merged into a dialogue subtitle.
- Currency symbols are written out (**dollár, font, euró**); never censor profanity that is audible — match its force in Hungarian.
- Use the published Hungarian title of any work referenced; if none exists, keep the original.

## 4. Marketing and transcreation

- **Tegezés is the modern consumer default** — it has spread through Hungarian advertising, retail, and media (the IKEA model). Choose **magázás** for conservative/premium/B2B/health/finance audiences and for older target groups. The choice is strategic; apply it to every asset in the campaign.
- **CTAs are short informal imperatives** in te-form: *Buy now* → **Vásárolj most** · *Add to cart* → **Tedd a kosárba** · *Download free* → **Töltsd le ingyen** · *Subscribe* → **Iratkozz fel**. Formal variant when the audience demands it: **Vásároljon most**. First-person button copy converts well: **Kérem a kupont!**
- Transcreate, don't translate: rebuild wordplay, rhyme, and cultural references with Hungarian material of equal force (the *teljes átalakítás* and *kompenzálás* operations — see `literary-translation.md` §6); keep claims and legal wording exact.
- Exclamation marks are tolerated in marketing far more than in UI copy — but one per thought, not English triple-stacking.
- Headlines follow sentence case (no Title Case), and slogans stay short: Hungarian words run long, so cut syllables, not meaning.
- Watch anglicism inflation in brand copy: *feedback* → **visszajelzés**, *deadline* → **határidő**, *meeting* → **megbeszélés** — unless the brand voice deliberately uses startup jargon.

## 5. Official, administrative, and legal prose (plain language)

Hungarian officialese (hivatali nyelv) has documented diseases; the EU clear-writing guide and the Budapest plain-language handbook prescribe the cures. When translating official English, produce clean administrative Hungarian, not a calque of bureaucratese:

- **Kill the kerül-passive:** *will be investigated* → **kivizsgálják** (not *kivizsgálásra kerül*); *was recognized* → **felismerték** (not *felismerésre került*). Same for empty *történik / valósul meg / eszközöl* (*Módosítást eszközöltek* → **Módosították**).
- **Unpack -ás/-és nominalization chains into verbs:** *carry out an evaluation* → **értékel** (not *értékelést végez*); *exercise control* → **ellenőriz**; *submit a declaration* → **nyilatkozik**.
- **Replace postposition sprawl with case suffixes:** *negotiations regarding roaming fees* → **tárgyaltak a roamingdíjakról** (not *…a roamingdíjak tekintetében*); treat **tekintetében, keretében, vonatkozásában, során** as red flags.
- **esetén / hiányában → ha-clauses addressed to the reader:** *in case of submission at the customer service desk* → **ha Ön az ügyfélszolgálaton nyújtja be**; *in the absence of consent* → **ha Ön nem járul hozzá**.
- **Speak to the reader as Ön, about your office as mi**; recast third-person abstractions: *The taxpayer is obliged to file…* → **Önnek akkor kell bevallást benyújtania, ha…**
- **One sentence, one idea** — at most ~20 words and 3 clauses; put the main message first, the reader's task second, and the statute reference **at the end, in parentheses**: *(az Art. 50. § (1) bekezdése alapján)*.
- **Legal citation format:** *50. § (1) bekezdés a) pont*; act titles: *2017. évi CL. törvény*; EU structure: *1. cikk, (2) bekezdés, II. melléklet* (unit nouns lowercase, singular even for several: *az (1) és a (2) bekezdésben*).
- Concrete over abstract: *employment opportunities* → **munkahelyek**; *negative development* → **csökkenés**.
- In genuinely legal instruments (contracts, statutes) precision outranks elegance: keep terms of art (*kártérítés* vs *kártalanítás*), keep defined terms consistent, and do not "improve" ambiguity away — flag it instead. The *-tatik/-tetik* passive and *által*-agent survive legitimately in this register only.
