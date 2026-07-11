---
name: interpreting-hungarian
description: Translates between English and Hungarian, in both directions, into idiomatic, native-sounding output rather than literal calque. Use whenever the user asks to translate, interpret, localize, or render text English→Hungarian or Hungarian→English — documents, emails, UI strings, marketing copy, subtitles, song lyrics, fiction, poetry, dialogue, official text, or a single word or phrase — and also when the user simply pastes text in one of the two languages and asks for the other. EN→HU covers what naive translation gets wrong (topic–focus word order, definite vs. indefinite conjugation, dropped pronouns and copula, English passives and -ing forms, coverb aspect, case suffixes, register te/ön, false friends, Hungarian punctuation and numbers), plus literary norms and domain conventions for UI, subtitles, marketing, official prose. HU→EN covers tense selection, articles, do-support, restored subjects and objects, name order, and English punctuation.
---

# Interpreting Hungarian: English ↔ Hungarian translation

Two directions, one standard: output a native would write, never a word-for-word calque. **The body of this file governs English → Hungarian.** For **Hungarian → English**, the load-bearing rules are in the [Hungarian → English section](#hungarian--english) below, and `reference/hungarian-to-english.md` holds the full system — read it before drafting in that direction.

English → Hungarian first. Hungarian organizes information around a pre-verbal focus position, drops what English makes explicit, conjugates verbs by the definiteness of their object, and glues onto the noun (as case suffixes) most of what English puts in front of it (as prepositions). A literal rendering looks grammatical but reads unmistakably foreign — Hungarian translation studies has a name for that failure mode: *kvázi-helyesség*, quasi-correct text where every sentence parses and the whole still sounds translated.

## Operating principle (read first)

You already translate English→Hungarian competently. Most sentences come out natural if you simply re-express the *meaning* instead of the words. So:

- **Default to your own fluent Hungarian.** Do not mechanically run every rule below on every sentence — that produces over-corrected, stilted output (e.g. forcing focus-movement, a coverb, or a dative-possessor construction where the plain version was already idiomatic). Over-application is as much a failure as calquing.
- **Reach for the rules as a diagnostic** when the English structure is actively pulling you toward a calque: passives, dummy *it*, *there is/are*, rigid SVO order, trailing adverbials, phrasal verbs, -ing clauses, prepositions, English punctuation, or ambiguous register.
- **The self-check at the end is a safety net**, not a per-sentence checklist. Apply it when a draft sentence still "feels English-shaped."
- **Calibrate depth to the text.** For a multi-paragraph, literary, or stylistically demanding passage, settle the register, the te/ön map of every speaking pair, names, titles, and recurring terminology *before* writing the first sentence. For a short everyday request, translate directly — deliberation there only produces over-corrected output; the only checks a one-liner needs are register and, if numbers appear, the *billió → milliárd* scale. For a long or technical text, also lock terminology: the same source term gets the same translation every time — elegant variation on defined terms is an error.
- **The deepest tell of translated text is what's *missing*.** Corpus research on translated Hungarian (the unique-items hypothesis; on the Pannónia Corpus *szokott* runs at roughly half its native frequency in translations) shows translations under-use the devices the source language gives no stimulus for — and over-use whatever has a direct English twin. So where one fits naturally, reach for the Hungarian-only inventory: *szokott*, coverb aspect, *-lak/-lek*, *hadd*, *tessék*, the dative possessor, the associative *-ék*, diminutives, discourse particles (*ugye, hát, ám, bezzeg, azért, is*). Never force one in; just stop the English from filtering them out.

### Route by text type

The reference files hold depth this file only sketches. Read the matching file **before drafting** whenever a row applies — not only when uncertain; the rules there are systematic, not stylistic taste:

| Text type | Read first | What it prevents |
|---|---|---|
| **Hungarian → English, any text type** | `reference/hungarian-to-english.md` | Hunglish word order, missing present perfect, missing articles and do-support, surname-first names, Hungarian punctuation residue |
| Fiction, poetry, drama, song lyrics, dialogue-heavy or voice-driven prose | `reference/literary-translation.md` | English quote-mark dialogue, tense backshift, wrong name/title handling, lost verse form, translationese |
| Software/UI strings, error messages, subtitles, marketing copy, official or legal prose | `reference/domain-conventions.md` | wrong register (te/ön), imperative buttons, subtitle limit violations, bureaucratese |
| A full conjugation, case, or postposition paradigm is needed | `reference/grammar-tables.md` | guessed inflection |
| Letters/emails, exhaustive false-friend or formatting lookup | `reference/style-lexicon.md` | wrong salutation, cognate traps |

Everyday English → Hungarian prose — a plain email, a paragraph, a phrase — needs no reference file; this file is self-sufficient for it.

## Method

1. Read the whole passage for meaning, tone, register, intent, and text type; route per the table above.
2. Hold the meaning; drop the English wording.
3. Re-express in Hungarian — freely restructure, split, or merge sentences around topic–focus–verb.
4. Read your Hungarian aloud; fix anything a native would not say.

---

## Word order and information structure

Neutral sentences — no special emphasis — are often the *same* order as English (subject–verb–object): *Éva szereti a virágokat.* (Eve likes the flowers.) · *Tamás eszi az almát.* (Tamás is eating the apple.) Don't reorder a sentence that is already neutral and natural. What breaks the English parallel:

**Trailing time/place adverbials.** English tacks them onto the end; Hungarian normally places them *before* the verb (and time before place). This is the single most common calque.
- Peter saw a cat in the garden yesterday.
- calque: *Péter látott egy macskát a kertben tegnap.*
- natural: **Péter tegnap a kertben látott egy macskát.**

**The pre-verbal focus slot.** Whatever is emphasized — the answer to an implicit *who/what/where?*, or an English *it was X that…* cleft — moves into the slot **immediately before the verb**, and any coverb is pushed *after* the verb. Hungarian has no *it*-cleft; don't translate "it was…that" literally.
- It was PÉTER who ate the apple. → **PÉTER ette meg az almát.** (neutral: *Péter megette az almát.*)
- It was the BOOK I read (not the paper). → **A könyvet olvastam el.**

**"only" = csak, and it moves with its focus.** A *csak*-phrase is inherently focused: *csak* stands directly before the word it restricts, and the whole phrase sits pre-verbally. English *only* hugs the verb regardless of scope; Hungarian placement changes the meaning.
- Only I saw the film. → **Csak én láttam a filmet.** · I saw only the film. → **Csak a filmet láttam.** · I only *saw* it (didn't buy it). → **Csak láttam.**

**Bare (article-less) object → S–O–V.** A non-specific object with no article often sits right before the verb and forms a unit with it: *Peter is writing a letter.* → **Péter levelet ír.** (vs. *Péter ír egy levelet*, which counts "a [single] letter").

**Quantifiers are not focus.** *minden* (every), *mindenki* (everyone), *mindig* (always), *sok* (many) sit pre-verbally but **keep the coverb attached** — unlike focus, they do not invert it.
- Everyone watched the film. → **Mindenki megnézte a filmet.** (not *…nézte meg…*)

**Questions take no do-support and no auxiliary inversion.**
- *Wh*-questions put the question word in the focus slot (coverb inverts): What is the boy eating? → **Mit eszik a fiú?** · Where are you going? → **Hová mész?**
- *Yes/no* questions keep statement order, marked by intonation; in formal/embedded use, the enclitic **-e** on the verb = "whether/if": Is he reading? → **Olvas?** · I don't know if he's coming. → **Nem tudom, hogy jön-e.**

## Negation, and the particles *is* / *sem*

- ***nem*** immediately precedes the verb (or the focus it negates) and, like focus, **pushes the coverb after the verb**: I didn't read it. → **Nem olvastam el.** (not *Nem elolvastam.*)
- **Negative concord is obligatory** — the "double negative" is correct. An n-word (*senki* nobody, *semmi* nothing, *soha* never, *sehol* nowhere) **must** co-occur with *nem*/*sem*: Nobody helps me. → **Senki nem segít nekem.** / **Senki sem segít nekem.** · I see nothing. → **Nem látok semmit.**
- ***nem* + 3rd-person *van*/*vannak* merges into *nincs* / *nincsenek*** (and *sincs* under *sem*): There is no coffee. → **Nincs kávé.** (never *nem van*).
- The negative imperative uses **ne**, not *nem*: Don't go! → **Ne menj!**
- ***is*** ("too/also") is an enclitic that **hugs the word it adds**, never floating to the clause end like English — and unlike focus it does not detach the coverb: I saw Peter too. → **Pétert is láttam.** · Peter came too. → **Péter is eljött.** (not *…jött el*). · Me too. → **Én is.**
- Under negation, *is* → ***sem*** ("either/neither"): I'm not coming either. → **Én sem jövök.** Scalar "even" = **még … is**: Even Peter came. → **Még Péter is eljött.**

## Drop what Hungarian does not need

- **Subject pronouns** — omit unless emphatic/contrastive: *It is raining.* → **Esik.** · *I love it.* → **Imádom.** · *She loves her job.* → **Szereti a munkáját.** (not *Ő szereti az ő munkáját*).
- **Copula *van/vannak*** — omit with predicate adjectives/nouns in the 3rd-person present: *The house is big.* → **A ház nagy.** (never *…nagy van.*) But **keep it for location and existence**: *The cup is on the table.* → **A csésze az asztalon van.** And it is **never dropped in the future**: *He will be a doctor.* → **Orvos lesz.** (not *Ő fog orvos lenni*).
- **There is/are** → sentence-initial **Van/Vannak**, never *Ott van*: *There is a book on the table.* → **Van egy könyv az asztalon.**
- **Indefinite article *egy*** — drop far more often than English *a/an*, especially before a predicate noun/profession: *I am a doctor.* → **Orvos vagyok.** (not *Egy orvos vagyok.*) *iOS is a popular platform.* → **Az iOS népszerű platform.** Keep *egy* only when it genuinely means "one / a certain": *I saw only one man.* → **Csak egy embert láttam.**
- **Redundant possessives** — the possessive suffix already marks the owner: *I washed my hands.* → **Megmostam a kezem.** (not *az én kezeimet*).
- **English *some/any* usually vanish** — they are grammar, not meaning: *Do you have any questions?* → **Van kérdése?** · *Would you like some coffee?* → **Kérsz kávét?** Translate them (*néhány, valamennyi, bármilyen*) only when the quantity or free choice is genuinely the point (*any of them* → **bármelyik**).

## Definite vs. indefinite conjugation

Match the verb to the **grammatical form** of its object (not its meaning). This is one of the most audible non-native errors.

| Object is… | Conjugation | Example |
|---|---|---|
| absent, or indefinite: *egy*, bare noun/plural, *sok/néhány/két*, **minden + N**, *valamit/valakit*, *mit/kit*, *semmit/senkit*, **and 1st/2nd-person pronoun objects** (*engem, téged, minket, titeket*) | **indefinite** | *Látok egy fát.* · *Fákat látok.* · *Mit látsz?* · *Látok valamit.* · *Ismerek minden titkot.* · *Látsz engem.* |
| definite: *a/az* + N, proper name, possessive-suffixed N, demonstrative (*ezt/azt a…*), 3rd-person pronoun (*őt, azt, őket*), reflexive (*magát*), *melyiket / mindegyiket / valamennyit / mind*, **a *hogy*-clause**, and **formal *önt*** | **definite** | *Látom a fát.* · *Látom őt.* · *Ismerem a titkodat.* · *Melyiket kéred?* · *Tudom, hogy jössz.* · *Látom Önt.* |

Cases a literal approach gets wrong:
- **1st/2nd-person object pronouns take the *indefinite* conjugation**, even though *me/you/us* feel definite: *You see me.* → **Látsz engem.**
- **But "I → you" has its own special form, *-lak/-lek*** — extremely common: *I love you.* → **Szeretlek.** · *I'm waiting for you.* → **Várlak.** · past: *I saw you.* → **Láttalak.** Used only when the subject is *I* and the object is *you*.
- **The quantifier trap:** *minden* (every), *mindenki* (everyone), *mindent* (everything) take the **indefinite** conjugation — *I know everyone here.* → **Mindenkit ismerek.** (not *ismerem*) — whereas *mindegyik / valamennyi / mind / az összes* (each/all) take the **definite**: *I'll take all of them.* → **Mindegyiket kérem.** A possessive suffix overrides this and forces **definite**: *I know your every secret.* → **Ismerem minden titkodat.**
- **Verbs of liking/knowing take a generic object with the definite article + definite conjugation**, where English uses a bare noun: *I like coffee.* → **Szeretem a kávét.** (not *Szeretek kávét.*)

Full paradigms (present/past, definite/indefinite, *-lak/-lek*): see `reference/grammar-tables.md`.

## Coverbs and aspect

Coverbs (*igekötők*: *meg, el, fel, le, be, ki, át, oda, vissza, rá, össze, szét*…) carry **direction** and **aspect**. A bare verb is imperfective/atelic (a process); a coverb usually makes it perfective/telic (completed, with a result). English often packs that completion into a particle ("eat **up**", "read **through**") or a result verb ("find", "kill") — Hungarian needs an explicit coverb, or it reads as unfinished.

| English (result/completion) | bare = wrong/atelic | native (coverb) |
|---|---|---|
| I read the (whole) book. | *Olvastam a könyvet.* ("was reading") | **Elolvastam a könyvet.** |
| I ate the apple (up). | *Ettem az almát.* | **Megettem az almát.** |
| I found my coat. | *Találtam a kabátomat.* (stumbled on) | **Megtaláltam a kabátomat.** |
| I passed the exam. | *Elmentem a vizsgán.* (= left) | **Átmentem a vizsgán.** |

Also turn phrasal verbs and idioms into coverb constructions, never word-for-word: *give up* → **felad**; *look for* → **keres**; *it's raining heavily* → **szakad az eső**. The traffic runs the other way too — do not add coverbs English phrasal particles seem to license when the bare verb is the Hungarian word: *install the software* → **telepíti a szoftvert** (not *feltelepíti*), *communicate* → **közöl / megbeszél** (not *lekommunikál*).

**Placement carries aspect and is the load-bearing rule:** the coverb is **pre-verbal (attached)** in neutral affirmatives and plain yes/no questions, and **post-verbal (separated)** under negation, focus, *wh*-questions, and the imperative.
- I found it. → **Megtaláltam.** · I didn't find it. → **Nem találtam meg.** · Find it! → **Találd meg!**

## English passive → Hungarian active or resultative

Hungarian has no generalized syntactic passive. Choose by what the English passive actually describes:

- **An action or event** (something happened; the agent is unstated) → **3rd-person-plural active**:
  - Mistakes were made. → **Hibákat követtek el.**
  - The door was opened. → **Kinyitották az ajtót.**
  - The newspaper was already read. → **Az újságot már elolvasták.**
- **A resulting state** (English *is/are* + participle, describing a condition) → the ***-va/-ve van* resultative**, the closest Hungarian equivalent of the English passive:
  - The door is locked. → **Az ajtó be van zárva.**
  - The screen is broken. → **A képernyő be van törve.**

Note the contrast: *the door was opened* (event) → **kinyitották**, but *the door is locked* (state) → **be van zárva**. Cautions: *-va/-ve van* only works with certain telic transitive verbs — when it sounds off, use the 3rd-plural active instead (*A könyvet megírták*, not *A könyv meg van írva*). Use a lexical middle/anticausative only where idiomatic (*eltörik* — breaks, *elromlik* — breaks down, *kinyílik* — opens); don't manufacture *-ódik/-ődik* forms as a generic passive. Avoid the archaic *-tatik/-tetik* passive outside deliberately literary or legal text — and never render a passive with the bureaucratic **kerül**-periphrasis: *the event will be held* → **megrendezik** (not *megrendezésre kerül*), *was created* → **létrehozták / jött létre** (not *lett létrehozva*).

## Generic "you" and "one"

English generic *you* is not *te*. Pick by nuance:

- **az ember** — the speaker generalizing lived experience: *You never know.* → **Az ember sosem tudhatja.**
- **3rd-person plural** — "people in general / they": *How do you say it in Hungarian?* → **Hogy mondják magyarul?** · *They say it works.* → **Azt mondják, működik.**
- **lehet / kell + infinitive** — possibility/necessity for anyone: *You can see the mountains from here.* → **Innen látni lehet a hegyeket.** · *How do you pronounce this?* → **Hogyan kell ezt kiejteni?**
- **1st-person plural** when the speaker is included: *You never know.* → **Sose tudhatjuk.**

A literal 2nd-person generic (*Sosem tudod…*) is colloquial-only and reads anglicized in neutral prose.

## English -ing forms

- **After verbs of liking/wanting/starting/knowing-how → infinitive:** *I like reading.* → **Szeretek olvasni.** (never *szeretek olvasást*).
- **As a full noun phrase — with an article, case suffix, or postposition → the -ás/-és noun:** *Smoking is harmful.* → **A dohányzás káros.** · *before leaving* → **indulás előtt** · *without knocking* → **kopogás nélkül**. A postposition can never govern an infinitive.
- **Bare-subject generalizations take either:** *Stealing is a crime.* → **Lopni bűn.** / **A lopás bűn.**
- **Participle clauses → a finite clause**, usually *miközben/amikor* (time) or *mivel/mert* (cause): *Walking home, he saw an old friend.* → **Miközben hazafelé sétált, meglátta egy régi barátját.** Reserve **-va/-ve** for manner accompanying the main verb (*She entered smiling.* → **Mosolyogva lépett be.**) and for states (**Az ajtó zárva van.**); it does not narrate events (*A macska fel van mászva a fára* is comic), and **-ván/-vén** is archaic — only for deliberate period style.

## English prepositions → Hungarian case suffixes and postpositions

English uses separate words *before* the noun (in, on, to, from, with, for); Hungarian uses **suffixes glued after** the noun, or **postpositions placed after** it. There is almost never a separate word for "in/on/to/from". Reaching for one is a major calque. Location is a **3×3 system**: interior / surface / proximity, each crossed with static / motion-to / motion-from.

| | in/at (static) | to/into (motion to) | from (motion from) |
|---|---|---|---|
| **interior** (inside) | -ban/-ben | -ba/-be | -ból/-ből |
| **surface** (on) | -on/-en/-ön | -ra/-re | -ról/-ről |
| **proximity** (by / at a person) | -nál/-nél | -hoz/-hez/-höz | -tól/-től |

Where Hungarian's choice **defies English intuition** (high-value traps):
- on the bus/train → **a buszon / a vonaton** (surface, not *-ban*); getting on → **felszállok a buszra**; getting off → **leszállok a buszról**.
- at the doctor's → **az orvosnál**; (going) to the doctor's → **az orvoshoz**; from the doctor's → **az orvostól** (a *person* takes the proximity series).
- in the picture → **a képen**; at the university → **az egyetemen**; in the street → **az utcán** (surface).
- Hungarian towns and "Hungary" take the **surface** series — in/to/from Budapest → **Budapesten / Budapestre / Budapestről**; in Hungary → **Magyarországon** — but foreign places take **interior**: in London / in Germany → **Londonban / Németországban**.

Other high-frequency mappings: object **-t** (*almát*); "to/for" + possessor **-nak/-nek** (*Péternek*); "with / by (means)" **-val/-vel** (*késsel, vonattal*); "about (a topic)" **-ról/-ről** (*a háborúról*); "for the sake of" **-ért** (*pénzért*); "until/for (duration)" **-ig** (*hat óráig*); "as (in the role of)" **-ként** (*tanárként*); "at (clock time)" **-kor** (*ötkor*). Note "for" splits (**-ért** / **-nak,-nek** / verb-governed **-ra,-re**: *várok rád*), and "with" splits into instrumental **-val/-vel** vs. the postposition **együtt**.

**Postpositions follow the noun** (most take the bare nominative): *az asztal alatt* (under the table), *a ház mögött* (behind the house), *ebéd után* (after lunch), *szerinted* (according to you), *nélküled* (without you). With a pronoun they take personal endings — **alattam** (under me), **szerintem** (in my opinion), **miatta** (because of it) — never *alatt én*.

**Demonstrative agreement** (very common error): in *this/that + noun*, the demonstrative takes the **same case** as the noun **and** the article *a/az* stays between them. The *-z* assimilates.
- in this house → **ebben a házban** (not *ez a házban*) · to that city → **abba a városba** · on this table → **ezen az asztalon** · about that film → **arról a filmről**.

**Time expressions** split four ways: clock time **-kor** (*ötkor*); days take superessive **-n** (*hétfőn*, *pénteken*; but *vasárnap* bare); months/years take inessive (*januárban*, *2020-ban*); parts of day are bare adverbs (*reggel*, *este*).

The full case inventory, place-name rules, and complete postposition tables (directional triples, case-governing ones, personal forms): see `reference/grammar-tables.md`.

## Tense, the future, and habits

Hungarian has only **past** and **present**. For the future, use the **present** for scheduled or certain events; reserve **fog + infinitive** for emphasis or uncertainty.
- I'll call you tomorrow. → **Holnap hívlak.** (present)
- It will probably rain. → **Valószínűleg esni fog.**

There is **no progressive aspect** — one present form covers "I read" and "I am reading"; mark ongoing action with **éppen/most** if needed: *I'm reading right now.* → **Éppen olvasok.** (never a *van* + participle construction).

**English present perfect + for/since → Hungarian PRESENT.** A state that still holds stays in the present tense; the past tense silently changes the meaning to "no longer true":
- I've lived here for two years. → **Két éve itt lakom.** — *Két éve itt laktam* means "I lived here two years **ago**."
- How long have you known him? → **Mióta ismered?** · She's been ill since Monday. → **Hétfő óta beteg.**
(A completed-event perfect is ordinary past: *I've finished it.* → **Befejeztem.**)

**Habitual "usually" = szokott + infinitive** — past-tense in form, **present-habitual in meaning**: *I usually drink coffee in the morning.* → **Reggel kávét szoktam inni.** Do not read it as "used to". English **used to** = past tense + a past time adverb (*Régen minden nap edzettem.* — I used to work out every day), or *régen* + *szokott*.

## Reported speech: no backshift, ever

Hungarian keeps the **tense of the original utterance**; only deictics shift (*ma → aznap*, *itt → ott*).
- He said he was tired. → **Azt mondta, hogy fáradt.** — *Azt mondta, hogy fáradt **volt*** asserts something else ("he said he **had been** tired").
- He said he would come. → **Azt mondta, hogy eljön / el fog jönni.** — *eljönne* would make it conditional ("would come if he could").
- She asked where I worked. → **Azt kérdezte, hogy hol dolgozom.**

## Conditional, "if"-clauses, and English "would"

- Present conditional = **-na/-ne/-ná/-né** (1sg indefinite is always **-nék**, never *-nák*). Past conditional = **past tense + invariant *volna***: I would have written. → **Írtam volna.**
- ***ha* ("if") puts the conditional in BOTH clauses** (English uses past in the *if*-clause, conditional only in the main one):
  - If I had money, I'd buy a car. → **Ha lenne pénzem, vennék egy autót.** (not *Ha volt pénzem…*)
  - If I had had money, I'd have bought a car. → **Ha lett volna pénzem, vettem volna egy autót.**
- English "would" is often **not** the Hungarian conditional:
  - past habit ("we would go every summer" = used to) → **past tense** or *szokott*: **Nyaranta a tengerhez jártunk.**
  - reported speech ("he said he would come") → **present/future**, no backshift (see above).
  - polite "I would like" → fixed **szeretnék**: *I'd like a coffee.* → **Szeretnék egy kávét.**

## Imperative / subjunctive and "want someone to…"

The imperative and subjunctive share the **-j-** form. The coverb goes **after** the verb (*Ülj le!* — Sit down!; *Ne ülj le!* — Don't sit down!). The big structural pitfall: English "want/ask/tell someone **to** do X" is **not** an infinitive in Hungarian when the subjects differ — it is **azt + hogy + subjunctive**:
- I want you to go. → **Azt akarom, hogy menj.** (not *Akarlak menni*)
- Tell him to come. → **Mondd meg neki, hogy jöjjön.**

(When the subject is the *same*, the infinitive is correct: *I want to go.* → **El akarok menni.**) "Let me/him…" = **hadd** + subjunctive (*Hadd lássam!*); "let's…" = the 1st-person-plural form (*Menjünk!*). Assimilation and irregular imperatives: see `reference/grammar-tables.md`.

## Modality (can / must / may / should / would like)

- **must / have to** = **kell** + **dative** + **inflected infinitive** (the infinitive itself takes a personal ending; *kell* stays invariant): I have to go. → **(Nekem) el kell mennem.** · Ági has to go. → **Áginak el kell mennie.** · past: **El kellett mennem.**
- **should / ought to** = **kellene / kéne** (+ inflected infinitive): You should study. → **Tanulnod kellene.**
- The dative + inflected infinitive pattern extends beyond *kell* to *nehéz, könnyű, sikerül, érdemes, muszáj*: It would be hard for an economist to answer this. → **Egy közgazdásznak nehéz lenne ezt megválaszolnia.** · I managed to open it. → **Sikerült kinyitnom.**
- English "can" splits: **tud** = learned ability / "know how" (*I can swim.* → **Tudok úszni.**); **-hat/-het** = possibility or **permission** (*May I sit down?* → **Leülhetek?**, not *Tudok leülni?*); **képes** = capable of (*Képes vagyok rá.*).
- **may / might / it's possible** → **-hat/-het** or **lehet (, hogy)**; **be allowed/forbidden** → **szabad / tilos** (*Szabad bejönni?* · *Tilos dohányozni.*).
- **"must not" ≠ "don't have to"** — English negates them alike; Hungarian splits them: *You must not smoke here.* → **Itt nem szabad dohányozni.** (prohibition) · *You don't have to come.* → **Nem kell eljönnöd.** (no obligation). Rendering *must not* as *nem kell* silently turns a ban into an option.

## The noun phrase

**Articles.** Hungarian uses the definite article *a/az* where English drops "the", and drops *egy* where English keeps "a":
- generic/abstract nouns take *a/az*: *I like music.* → **Szeretem a zenét.** · *Love is wonderful.* → **A szerelem csodálatos.**
- possessed nouns and body parts take *a/az*: *my book* → **a könyvem**; *My head hurts.* → **Fáj a fejem.**
- superlatives take *a/az*: *the best* → **a legjobb**.
- a demonstrative requires the article: *this chair* → **ez a szék** (not *ez szék*).
- rivers/lakes/mountains take it: **a Duna, a Balaton, a Kárpátok**; most countries/towns/people do **not**: *Magyarország, Budapest, Károly* — but plural/compound country names do: **az Egyesült Államok, a Cseh Köztársaság, a Fülöp-szigetek**.
- *a/az* is chosen by **sound**, not spelling: *a ház*, *az alma*, *az USA* (read with an initial vowel).

**Number.** After a numeral or quantifier the noun stays **singular** (the quantity is already marked): two cats → **két macska** (not *macskák*); many people → **sok ember**; every child → **minden gyerek**; both books → **mindkét könyv** (*mindkét* included — never plural after it).
- **Paired body parts are singular**: *My eyes hurt.* → **Fáj a szemem.** One of the pair = **fél**: *with one eye* → **fél szemmel**; *one-eyed* → **félszemű**.
- **Collective nouns take singular verbs**: *The police are investigating.* → **A rendőrség nyomoz.** (never plural agreement).
- **"One of the (most) X" = az egyik + leg- + singular**: *one of the best films* → **az egyik legjobb film** (never plural; elevated variant: *egyike a legjobb filmeknek*).
- **"The Smiths" (the family) = the associative -ék**: **Smithék** · *at the Smiths'* → **Smithéknél** · *my mum and them* → **anyámék**. (Formal alternative: *a Smith család*.)
- **Countability mismatches**: English mass nouns are ordinary countable nouns in Hungarian — *a piece of advice* → **egy tanács** (never *egy darab tanács*); *news* → **hír / hírek** (*That's great news!* → **Ez nagyszerű hír!**); *information* → **információ(k)**; *furniture* → **bútor(ok)**. Drop the English partitive scaffolding (*piece of, item of*) entirely.

**Adjectives.** An attributive adjective (before the noun) does **not** agree; a predicative one (after "to be") **does**: *red apples* → **piros almák** (singular *piros*) but *The apples are red.* → **Az almák pirosak.** Adjectives from place names are lowercase: *budapesti, vidéki*.

**Comparison.** Comparative = **-bb/-abb/-ebb**, superlative = **leg-** + comparative (with *a/az*): *faster* → **gyorsabb**; *the fastest* → **a leggyorsabb**. Irregulars: *jó→jobb, nagy→nagyobb, sok→több, kicsi→kisebb, szép→szebb*. "Than" = **-nál/-nél** *or* **mint + nominative** (never accusative): *taller than me* → **magasabb nálam** / **magasabb, mint én** (not *mint engem*). "As…as" = **olyan … mint**. Never calque "more X" as two words — it is one suffixed word (*szebb*, not *több szép*).

**Possession.** Possessor first, with the possessive suffix on the *possessed* noun: *Peter's book* → **Péter könyve**; *the window of the house* → **a ház ablaka**. The emphatic/disambiguating form uses the **dative**: **Péternek a könyve** (obligatory with demonstratives: *annak a háznak az ablaka*).

**"Have"** — there is **no verb "to have"**. Possession = **dative possessor + *van/nincs* + possessed noun with a possessive suffix**:
- I have a dog. → **Van egy kutyám.** · I have no money. → **Nincs pénzem.** · Peter has a car. → **Péternek van autója.** · I have friends. → **Vannak barátaim.**

**English noun strings.** Rebuild them; never stack spaced nouns. The workhorses: a solid compound (*climate conference* → **klímakonferencia**), the **-i adjective + noun** pattern (*customer service department* → **ügyfélszolgálati osztály**), or a possessive structure (*the head of the department* → **az osztály vezetője**). Compounds are written **solid** (*ügyfélszolgálat*, not *ügyfél szolgálat*); the 6-syllable/3-element hyphen rule: `reference/grammar-tables.md`.

**English right-branching → Hungarian left-branching.** English hangs modifiers *after* the noun (relative clauses, participles, *of*-phrases); Hungarian builds them *before* it with participial premodifiers: *the man standing at the door* → **az ajtóban álló férfi**; *the report published last week* → **a múlt héten közzétett jelentés**; *a solution acceptable to everyone* → **egy mindenki számára elfogadható megoldás**. When the premodifier grows heavy (several clauses' worth), fall back to a relative clause (*a férfi, aki…*) — stacked left-branching modifiers are the tapeworm sentences of officialese.

Possessive suffix paradigms and the *-é* form (*Ez a könyv Péteré.*): see `reference/grammar-tables.md`.

## Relative clauses: aki / amely / ami / amelyik

- **aki** for people; **amely** for things in formal writing; **ami** for things in neutral and spoken register — in dialogue *amely* sounds starched. Companies and institutions are things: *the firm that…* → **a cég, amely/ami…** (not *aki*).
- **ami is obligatory** when the antecedent is a whole clause or an unnamed pronoun: *He was late, which annoyed everyone.* → **Elkésett, ami mindenkit bosszantott.** (*amely* here is an outright error) · *They do all they can.* → **Megtesznek mindent, amit csak tudnak.**
- **amelyik** picks one out of a known set: *the mug that's blue* → **az a bögre, amelyik kék**.
- A comma always precedes the relative clause.

## Register: te / ön / maga / tetszik

Hungarian forces a formality choice English lacks. Keep it **consistent** across the whole text (pronouns, verbs, possessives, imperatives).

| Context | Choice | Verb agreement |
|---|---|---|
| casual: friends, peers, children, family | *te / ti* | 2nd person |
| professional, public, formal — the safe default | *ön / önök* | **3rd person** (*Ön tudja*) |
| *maga / maguk* | **avoid in formal writing** — can sound cold or rude; never to an elder/superior | 3rd person |
| warm deference (to elders) | *tetszik* + infinitive | *Hogy tetszik lenni?* |

A formal pronoun therefore takes a 3rd-person verb: *You (formal) speak Hungarian.* → **Ön beszél magyarul.** (not *Ön beszélsz*). Soften commands to *ön* with the conditional or *legyen szíves*: *Close the window.* → **Becsukná az ablakot?** / **Legyen szíves becsukni az ablakot.**

**Domain defaults** (full rules in `reference/domain-conventions.md`): software UI, documentation, and official text → **ön or impersonal phrasing, never te** (exceptions: children's products, AI-assistant prompt templates); consumer marketing → **te** unless the brand or audience is conservative/B2B; fiction and subtitles → assign per relationship between the characters, and keep each pair's choice stable. When the register of a plain text is genuinely ambiguous, default to **ön/önök**. Greetings, sign-offs, and salutation punctuation: `reference/style-lexicon.md`.

## Punctuation, capitalization, dates, and numbers

These are absent from English source text and are a major tell of machine translation. Apply them across the **entire output** — every sentence, not just the first occurrence. Leave code, URLs, and placeholders untouched.

- **Quotation marks:** Hungarian uses **„low-opening and high-closing”** — **„idézet”**, not English "…". Nested quotes use reversed guillemets: **„kint »bent« kint”**. In prose fiction, dialogue takes dashes instead — see the literary section below.
- **Dashes:** Hungarian does not use the em dash. Ranges take an **unspaced en dash** (*1995–2005*, *9–12. oldal*, *Budapest–Bécs*); the **spaced en dash** is the *gondolatjel* (parenthetical dash, dialogue dash); approximate values take a plain hyphen (*egy-két nap* — a day or two).
- **Decimal comma, space thousands:** `1,234.56` → **1 234,56**; percent attaches with **no space**: `3.5%` → **3,5%** (suffixed: *25%-os, 6%-kal*). Currency unit follows, after a space: **1 000 Ft**, **20 €**.
- **Dates are descending with periods:** *June 13, 2026* → **2026. június 13.** (lowercase month, trailing period). "On [date]" attaches a suffix and drops the period: **2026. június 13-án**; "on the 1st" → **1-jén**. No period in possessive/postpositional year phrases: **2026 októberében**, **2026 óta**. Decades: **a ’90-es évek**.
- **Capitalization is far lighter than English** — lowercase for months, days, languages, nationalities, holidays, and "I": *I speak English and German.* → **Beszélek angolul és németül.** Headings and titles use sentence case: *Privacy Policy* → **Adatvédelmi irányelvek**. In letters, the polite **Ön** is capitalized as a courtesy.
- **Commas:** always put a comma before **hogy** and before clause-introducers **aki/ami/amely/mert/ha/mint** (even where English omits it): *I think that it's good.* → **Azt gondolom, hogy jó.** Do **not** put a comma before **és/vagy** joining a simple list: **kenyér, tej és tojás**.
- **Suffix on a numeral/acronym/foreign word via a hyphen:** **5-kor** (at 5), **EU-ban** (in the EU), **20%-kal** (by 20%), **Windows-szal** (with Windows). The suffix matches the **pronounced** form, assimilation included: **1-gyel** (*eggyel*), **2-vel**, **100-zal** (*százzal*).
- **"Billion" = *milliárd* (10⁹), not *billió*** (which is 10¹², i.e. "trillion") — a catastrophic error in finance: *$5 billion* → **5 milliárd dollár**. Use the **24-hour clock** (*14.30*; colloquial *fél 8* = 7:30).

Full formatting rules and worked examples: see `reference/style-lexicon.md`.

## Vowel harmony

Every suffix must harmonize with its stem: back-vowel stems take back suffixes (*ház-ban*), front-vowel stems take front (*kert-ben*), with front-rounded variants where they exist (*-hoz / -hez / -höz*, *-on / -en / -ön*). The vowels *i, í, e, é* are neutral — some stems containing only these still take **back** suffixes (*híd → hidak*, *férfi → férfiak*, *cél → célok*), so follow the attested form rather than guessing. Note also the **-val/-vel** assimilation: after a consonant the *v* assimilates and the consonant doubles (*busz → busszal*, *kés → késsel*, *vonat → vonattal*). A single disharmonic suffix marks the text as non-native.

## False friends

| English | wrong (what the cognate means) | correct |
|---|---|---|
| sympathetic | *szimpatikus* (likeable) | **együttérző** |
| actually | *aktuálisan* (currently) | **valójában / tulajdonképpen** |
| actual | *aktuális* (current, topical) | **tényleges / valódi** |
| eventually | *eventuálisan* (possibly, contingently) | **végül / végül is** |
| sensitive | *szenzitív* is OK; beware *szenzibilis* | **érzékeny** |
| sensible | *szenzibilis* | **értelmes / ésszerű** |
| realise | *realizál* (implement / book a profit) | **rájön / felismer** |
| novel (book) | *novella* (short story) | **regény** |
| concrete (material) | *konkrét* (specific) | **beton** |
| map | *mappa* (folder) | **térkép** |
| solid | *szolid* (modest, restrained) | **szilárd / masszív** |
| simple | *szimpla* (single, plain) | **egyszerű** |
| receipt | *recept* (recipe) | **nyugta / blokk** |
| sodium | *szóda* (soda water) | **nátrium** |
| **billion** | *billió* (= 10¹², trillion) | **milliárd** |

Extended list (transparent/transzparens, massive/masszív, gimnázium, konfekció, etc.): see `reference/style-lexicon.md`.

## One English verb, two Hungarian verbs

English collapses distinctions Hungarian keeps separate — pick by meaning, not by the dictionary's first entry:

- **know** = **tud** (facts, skills) vs **ismer** (people, places, works): *I know him.* → **Ismerem.** · *I know (that) he's here.* → **Tudom, hogy itt van.** · *I know Budapest well.* → **Jól ismerem Budapestet.**
- **like** = **tetszik** (spontaneous appeal — dative experiencer) vs **szeret** (habitual liking, love): *I like your dress.* → **Tetszik a ruhád.** (not *Szeretem a ruhádat*, which claims attachment) · *I like coffee.* → **Szeretem a kávét.**
- **stop** = **megáll** (halt) vs **abbahagy / leszokik** (cease an activity / quit a habit): *He stopped to smoke.* → **Megállt, hogy rágyújtson.** · *He stopped smoking.* → **Leszokott a dohányzásról.**
- **meet** = **találkozik** (encounter) vs **megismerkedik** (meet for the first time): *We met in 2010.* (first acquaintance) → **2010-ben ismerkedtünk meg.**
- **wear** — the native pattern is **rajta van**, not a verb: *She was wearing a red dress.* → **Piros ruha volt rajta.** (*viselt* is formal/police-report register).
- **play** an instrument, sport, or game = a **denominal verb** (*-zik* and kin), not *játszik + N*: *Do you play tennis?* → **Teniszezel?** (not *Játszol teniszt?*) · *She plays the piano.* → **Zongorázik.** · *plays chess/football/the drums/the violin* → **sakkozik / focizik / dobol / hegedül**. (*játszik* survives in "play a game/match of": *játszottunk egy parti sakkot*.)

**Body-state and situation traps** — English *be + adjective* is often a verb or a possessive construction in Hungarian:

- *I'm cold.* → **Fázom.** · *My feet are cold.* → **Fázik a lábam.** (never *Hideg vagyok*)
- *I'm hot.* → **Melegem van.** — never *Meleg vagyok*, which states sexual orientation, not temperature.
- *I'm late. / Sorry I'm late.* → **Elkéstem. / Bocsánat, hogy késtem.** (not *késő vagyok* — *késő* is the hour, not the person)
- *I'm hungry/thirsty/sleepy.* → **Éhes/szomjas/álmos vagyok.** (these three are adjectives — the trap is assuming the pattern generalizes)
- *It's cold (in here).* → **Hideg van (idebent).** — weather/ambient states take **van**.

## Light-verb collocations and calqued clichés

English "make/take/do + noun" rarely maps to *csinál*. Use the Hungarian light verb:
- make a decision → **döntést hoz** / **dönt** (not *döntést csinál*)
- take a photo → **fényképet készít** / **fotót csinál** (not *fotót vesz*)
- make a mistake → **hibát követ el** · ask a question → **kérdést tesz fel** · make a promise → **ígéretet tesz**
- spend time → **időt tölt** (but spend money → **pénzt költ**) · make sense → **van értelme** (not *értelmet csinál*)

And fixed social formulas, not literal calques: *Have a nice day!* → **Szép napot (kívánok)!** · *Please find attached…* → **Mellékelten küldöm…** · *I look forward to your reply.* → **Várom a válaszát.** · *Feel free to call me.* → **Hívj nyugodtan! / Hívjon nyugodtan!** (never *érezd szabadnak magad…*) · *I'm so excited!* → **Alig várom! / Már nagyon várom!** (*izgatott vagyok* is the spreading anglicism) · *Enjoy!* → **Jó szórakozást!** (meal: **Jó étvágyat!**) · *I forgot my umbrella at home.* → **Otthon hagytam az esernyőmet.** (Hungarian "leaves" things, it doesn't "forget" them somewhere) · *I can't help laughing.* → **Muszáj nevetnem. / Nem tudom megállni nevetés nélkül.** (the MT classic *nem tudok segíteni nevetve* is the failure this whole skill exists to prevent).

## Literary and creative texts

Read `reference/literary-translation.md` **before drafting** any fiction, poetry, drama, song lyrics, or voice-driven prose — it holds the műfordítás norms (Kosztolányi's tradition: the result must stand as Hungarian literature), the transfer-operation toolbox, and the translationese sweep. The five rules most often violated without it:

1. **Prose dialogue uses dashes, not quotation marks.** Every `"…," she said` becomes a new paragraph opened by a gondolatjel; the sentence-final period is dropped before the tag (but `?`/`!` are kept), and the tag runs lowercase:
   **– Szia – mondta Péter. – Gyere be!**
2. **No tense backshift** in narration or reported thought (see the reported-speech section) — English past-perfect chains collapse into the one Hungarian past, ordered by *mire*, *miután*, *már*.
3. **Names stay foreign in adult fiction** (Hans Castorp remains Hans Castorp); children's and fantasy literature Hungarianizes *speaking* names creatively (the Micimackó–Roxfort tradition).
4. **Published Hungarian titles are obligatory** when referencing works: *A Gyűrűk Ura*, *Rómeó és Júlia*, *Rozsban a fogó*.
5. **Verse translates form too** — the Hungarian norm is *formahű* (meter and rhyme both); song lyrics must stay singable.

## Hungarian → English

Read `reference/hungarian-to-english.md` **before drafting** any Hungarian→English translation — it holds the direction-specific system (tense selection, articles, information structure, names, register compensation, punctuation, the Hunglish tell list). The six rules most often violated without it:

1. **Re-encode the word order, don't copy it.** English is rigid SVO — the English sentence often starts in the *middle* of the Hungarian one. Hungarian pre-verbal focus → an English cleft, passive, or *only/even*: *PÉTER ette meg az almát.* → **It was Peter who ate the apple.** Trailing adverbials move back to the English end: *Péter tegnap a kertben látott egy macskát.* → **Peter saw a cat in the garden yesterday.**
2. **One Hungarian past fans out into four English pasts — and Hungarian present is often English present perfect.** *Már két éve itt lakom.* → **I've lived here for two years.** · *Megjött a vonat?* → **Has the train arrived?** Reported speech **backshifts**: *Azt mondta, hogy fáradt.* → **He said he was tired.**
3. **Restore what Hungarian drops**: subjects and dummy subjects (*Esik.* → **It's raining.** · *Van egy könyv az asztalon.* → **There is a book on the table.**), objects encoded only in the definite conjugation (*Látom.* → **I can see it/him/her.**), articles (*Orvos vagyok.* → **I'm a doctor.**).
4. **English negation is single and questions need do-support.** *Senki nem segít.* → **Nobody helps.** (never *Nobody doesn't help*) · *Nem látok semmit.* → **I can't see anything.** · *Szereted a kávét?* → **Do you like coffee?**
5. **Names flip to given-name-first**: *Nagy Éva* → **Éva Nagy**; established English forms of historical figures are obligatory (*Liszt Ferenc* → **Franz Liszt**).
6. **Convert punctuation and numbers to English conventions throughout**: „…” → "…", fiction dialogue dashes → quotation marks, decimal comma → point (*3,5%* → *3.5%*), *2026. június 13.* → *13 June 2026* / *June 13, 2026*, capitalize months, days, languages, nationalities, and *I* — and *milliárd* → **billion**, *billió* → **trillion**.

## Output format

Apply these rules to **every** translation in the conversation, at every length:

- Return **only the translation** (Hungarian for EN→HU, English for HU→EN) — no commentary, no romanization, no notes on your choices. Exceptions, exhaustively: the user explicitly asks for explanation; or a single word/short phrase is genuinely ambiguous, in which case give each reading with a one-word label in the target language: *table → asztal (bútor) / táblázat (adat)*.
- **Single word / short phrase:** give the equivalent only — no sentence, no preamble.
- **Longer text:** preserve the source's structure — paragraph breaks, lists, headings, bold/italic. Convert punctuation, quotes, numbers, dates, and fiction dialogue to the **target language's** conventions throughout — every sentence, not just the first occurrence.
- Leave brand names, code, URLs, and placeholders unchanged; translate *around* a placeholder so the sentence stays grammatical (EN→HU: use **a(z)** where an unknown value needs an article).
- Register, EN→HU: an explicit user instruction (*informal / te*, *formal / ön*) overrides everything; otherwise use the domain defaults above; when genuinely ambiguous, use **ön/önök** — without announcing the choice. HU→EN: the te/ön distinction dies — compensate with tone and forms of address per `reference/hungarian-to-english.md`.

## Model calibration

Written for Claude Sonnet 5, Claude Opus 4.8, and GPT-5.5; works unchanged on other models. Whichever you are:

- **Claude Sonnet 5 / Opus 4.8:** default reasoning depth is right for everyday texts. Deliberate more only where the operating principle directs it — long, literary, or multi-register passages (settle register, the T/V map, names, and terminology before drafting). Do not extend thinking on short requests; over-deliberation is what produces over-corrected, stilted output.
- **GPT-5.5:** the absolutes in this skill (**never** the *kerül*-passive, **only** the Hungarian translation, register consistent) are true invariants — apply them literally. Everything phrased as "default", "prefer", or "where natural" is a decision rule: judge by the outcome (would a native write this sentence?), not by rule coverage. Do not narrate rule application.
- **All models:** the routing table's "read before drafting" is literal — actually open the reference file; do not translate literary, domain, or HU→EN text from this file alone.

## Self-check (run when a sentence still feels English-shaped; HU→EN has its own list in `reference/hungarian-to-english.md`)

1. Would a native say this, unprompted?
2. Removed unnecessary *azt / őt / egy / van* and redundant pronouns/possessives? Generic "you" rendered with *az ember* / 3rd-plural / *lehet*, not *te*?
3. Emphasized element immediately before the verb? Time/place adverbials moved off the end (time before place)? *csak* directly before what it restricts?
4. Coverb in the right place — attached when neutral, **after the verb** under negation/focus/question/imperative — present where English implies completion (*megtaláltam*, not *találtam*), and absent where the bare verb is the word (*telepít*, not *feltelepít*)?
5. Conjugation correct for every verb — definite vs. indefinite (incl. *minden/mindenki* → indefinite, *hogy*-clause → definite, 1st/2nd-person objects → indefinite, the I→you *-lak/-lek*)?
6. English prepositions rendered as the right **case suffix or postposition** (3×3 spatial series; *a buszon*, *az orvoshoz*), with demonstrative agreement (*ebben a házban*)?
7. English passives → 3rd-plural active (*kinyitották*), or *-va/-ve van* where they describe a state (*be van zárva*) — and no *kerül*/*lett* periphrasis?
8. -ing forms resolved — infinitive after verbs, *-ás/-és* under articles/cases/postpositions, participle clauses as finite clauses?
9. "Have" as *van/nincs* + dative + possessive suffix? Numerals + **singular** noun? Paired body parts singular (*fáj a szemem*)? Attributive adjective **not** pluralized? *az egyik legjobb film* singular?
10. *ha*-clauses with the conditional in **both** clauses? "Want sy to…" as *hogy* + subjunctive? "Must" as *kell* + dative + inflected infinitive? Reported speech **not** backshifted? Present-perfect states in the **present** (*két éve itt lakom*)? *must not* as **nem szabad**, not *nem kell*?
11. Relative pronouns right — *aki* people, *ami* after whole clauses (obligatory), *amely* only in formal writing?
12. Register (te/ön) consistent, appropriate to the domain, with 3rd-person verbs for *ön*?
13. Hungarian punctuation applied to the whole text — „quotation marks” (or dialogue dashes in fiction), decimal comma, **3,5%**, **2026. június 13.**, unspaced en-dash ranges, lowercase months/days/nationalities, comma before *hogy*, *billion → milliárd*?
14. Vowel harmony correct on every suffix?
