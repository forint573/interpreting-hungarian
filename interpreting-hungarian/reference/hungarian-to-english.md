# Hungarian → English translation (reference)

Read this file **before drafting** any Hungarian→English translation, whatever the text type. The failure mode in this direction is **Hunglish**: English words arranged in Hungarian information structure, with Hungarian tense logic, missing articles, and Hungarian punctuation showing through. Every rule in the core `../SKILL.md` still applies — run it in reverse: what Hungarian drops, English requires; what Hungarian glues on, English puts in front; what Hungarian leaves to context, English marks with tense and articles.

Working stance (same as EN→HU): translate the meaning, not the words; the English sentence often starts in the *middle* of the Hungarian one. Drop pure filler (*hát, szóval, izé, ugyebár*) rather than translating it — but carry its force where it does real work (§9). Pick **one English variety** and hold it: US by default; UK when the audience, brief, or source conventions say so (date format, *-ise/-ize*, quote punctuation, *at the weekend* follow the choice).

## 1. Word order: re-encode the information structure

English is rigid SVO and marks emphasis with constructions, not position. Do not copy the Hungarian order; identify what the pre-verbal slot was doing and pick the English device for it:

| Hungarian device | English device | Example |
|---|---|---|
| neutral topic–comment | plain SVO, adverbials at the end (place before time) | *Péter tegnap a kertben látott egy macskát.* → **Peter saw a cat in the garden yesterday.** |
| pre-verbal focus | ***it*-cleft**, or stress-bearing *only/even/actually* | *PÉTER ette meg az almát.* → **It was Peter who ate the apple.** |
| focused object, agent irrelevant | **passive** (keeps the Hungarian topic as English subject) | *A jelentést már elküldték.* → **The report has already been sent.** |
| *csak*-phrase | *only* directly before the focused word | *Csak a filmet láttam.* → **I only saw the film. / I saw only the film.** |
| topicalized non-subject | keep an English subject; do not front the object | *A könyvet Péter írta.* → **The book was written by Peter. / Peter wrote the book.** (never *The book Peter wrote.*) |
| verb-initial existential/presentative | *there is/are*, *once upon a time* | *Volt egyszer egy király.* → **Once upon a time there was a king.** |

**The reassembly procedure** (the working method Hungarian translator training teaches): identify the Hungarian sentence's elements — subject, predicate, object(s), adverbials — then place them into the fixed English slots: **subject – (frequency adverb) – verb – indirect object – direct object – manner – place – time**. Only a time adverbial (or a contrastively fronted place phrase) may move to the head of the sentence.

- Adverbials at the end run **Manner–Place–Time**: *Tegnap este kedvesen rámosolygott Joe-ra a táncteremben.* → **She smiled at Joe kindly in the dance hall yesterday evening.** / **Yesterday evening, she smiled at Joe kindly in the dance hall.**
- Frequency adverbs sit between subject and verb (after the first auxiliary if there is one): *Sosem járok moziba.* → **I never go to the cinema.** · *Mindig éhes vagy.* → **You are always hungry.**
- Recipient before thing: *Küldtem neki egy levelet.* → **I sent her a letter.** (*I sent a letter to her* only to stress the recipient.)
- Same-subject purpose clause → **to-infinitive**: *Mari hazament, hogy aludjon.* → **Mary went home to sleep.** (not *so that she could sleep*).
- **Preserve what *is* marks.** Hungarian *is* attaches unambiguously to one word; English *too/also* floats, so anchor it: *Én is láttam.* → **I saw it too.** (me as well) · *Azt is láttam.* → **I saw that one too / I also saw that.** (that as well). When writing allows ambiguity, restructure (**so did I**, **as well as…**).
- **Dismantle the baroque period.** Hungarian academic and official prose nests subordinate clauses several layers deep; translated linearly it collapses into noise. Find the main clause first, give every clause its own strict internal order, and split freely — one flowing Hungarian period is often two or three clean English sentences. When subjects match, a participle smooths the seam: *Amikor meghallottam a csengőt, ajtót nyitottam.* → **Hearing the bell, I opened the door.**

## 2. Tense: one Hungarian past fans out, and present isn't always present

The single most consequential decision in this direction. Choose by the event's shape, not the Hungarian form:

| Hungarian signal | English tense | Example |
|---|---|---|
| narrative sequence of completed events (coverb-perfective) | **past simple** | *Tegnap megírtam a levelet.* → **I wrote the letter yesterday.** |
| backgrounded ongoing action (*éppen*, bare imperfective verb) | **past continuous** | *Éppen olvastam, amikor csöngettek.* → **I was reading when the doorbell rang.** |
| earlier-than-past (*mire, miután, már* + past) | **past perfect** | *Mire megérkeztem, már elment.* → **By the time I arrived, he had already left.** |
| past event with present relevance/result (*már, még nem*, no time adverb) | **present perfect** | *Megjött a vonat?* → **Has the train arrived?** · *Még nem ettem.* → **I haven't eaten yet.** |
| **present + *már/óta/X ideje*** (state still holding) | **present perfect (continuous)** | *Már két éve itt lakom.* → **I've lived / I've been living here for two years.** · *Hétfő óta beteg.* → **He's been ill since Monday.** |
| present for scheduled future (*holnap, jövőre* + present) | ***will* / *going to* / present continuous** | *Holnap megyek Bécsbe.* → **I'm going to Vienna tomorrow.** |
| *szokott* + infinitive | **simple present (+ usually)** | *Reggel kávét szoktam inni.* → **I usually drink coffee in the morning.** |
| *régen* + past (lapsed habit) | **used to** | *Régen sokat olvastam.* → **I used to read a lot.** |

- ***Két éve* is ambiguous — the verb decides.** With a punctual event it means **ago**; with a state it means **for**: *Két éve láttam.* → **I saw him two years ago.** · *Két éve itt lakom.* → **I've lived here for two years.** Misreading one for the other is a silent meaning change.
- **Reported speech backshifts** (the exact reverse of the EN→HU rule): *Azt mondta, hogy fáradt.* → **He said he was tired.** · *Azt mondta, hogy eljön.* → **He said he would come.**
- **Conditionals un-double**: Hungarian conditional in both clauses → English past in the *if*-clause only: *Ha lenne pénzem, vennék egy autót.* → **If I had money, I'd buy a car.** · *Ha lett volna időm, elmentem volna.* → **If I'd had time, I would have gone.**
- **"Want someone to…"**: *Azt akarom, hogy menj.* → **I want you to go.** (infinitive, not a *that*-clause).
- Perception verbs prefer *can*: *Látom.* → **I can see it.** · *Hallak.* → **I can hear you.**

## 3. Restore what Hungarian drops

- **Subjects, including dummies**: *Esik.* → **It's raining.** · *Késő van.* → **It's late.** · *Van egy könyv az asztalon.* → **There's a book on the table.** · *Öten voltunk.* → **There were five of us.**
- **Objects encoded in the definite conjugation**: *Tudom.* → **I know (it).** · *Megtaláltad?* → **Did you find it?** — supply *it/him/her/them* from context.
- **Articles**: *Orvos vagyok.* → **I'm a doctor.** (indefinite article before professions/predicate nouns). Generic *a/az* disappears: *A szerelem csodálatos.* → **Love is wonderful.** · *Szeretem a zenét.* → **I love music.** But rivers, seas, mountain ranges, plural countries keep *the*: *a Duna* → **the Danube**, *az Egyesült Államok* → **the United States**.
- **Possessives English requires**: *Megmostam a kezem.* → **I washed my hands.** · *Fáj a fejem.* → **I have a headache.** · *Megvan a jegyed?* → **Do you have your ticket?**
- **Plurals after numerals**: *két macska* → **two cats** · *sok ember* → **many people** · *öt éve* → **five years ago**.
- **Paired body parts go plural**: *Fáj a szemem.* → **My eyes hurt.** (singular only if genuinely one: *fél szemmel* → **with one eye**).

## 4. Negation, questions, agreement

- **Negative concord → single negation** with the *any*-series: *Senki nem segít.* → **Nobody helps. / No one is helping.** · *Nem látok semmit.* → **I can't see anything.** · *Soha nem jár ide.* → **He never comes here.**
- ***nincs*** → *there is no / doesn't have*: *Nincs kávé.* → **There's no coffee.** · *Nincs pénzem.* → **I don't have any money. / I have no money.**
- **Do-support and inversion**: *Szereted a kávét?* → **Do you like coffee?** · *Hol dolgozol?* → **Where do you work?** — an intonation-only Hungarian question still needs full English question syntax.
- **The -e particle** → *whether/if*: *Nem tudom, hogy jön-e.* → **I don't know whether he's coming.**
- ***Ugye*** → **tag question**: *Ugye szereted?* → **You like it, don't you?** · *Ugye nem felejtetted el?* → **You haven't forgotten, have you?**
- **Agreement**: 3sg **-s** on every present verb; *a rendőrség nyomoz* → **the police are investigating** (*police* is plural-only); *a csapat nyert* → **the team won** (UK also *the team have won* — follow the variety); family: *Smithék* → **the Smiths**.
- **Countability, reversed**: *információk* → **information** (singular, no *informations*); *tanácsok* → **advice** (*egy tanács* → **a piece of advice**); *hírek* → **news** + singular verb (*Ez nagyszerű hír!* → **That's great news!**); *bútorok* → **furniture**.

## 5. Cases and postpositions → prepositions

Unpack every suffix into the right preposition — by meaning, not by the 3×3 grid: *a buszon* → **on the bus**, but *a képen* → **in the picture**, *az utcán* → **in the street** (UK) / **on the street** (US), *az égen* → **in the sky**. Time: *hétfőn* → **on Monday**, *ötkor* → **at five**, *januárban* → **in January**, *nyáron* → **in summer**, *hétvégén* → **at the weekend** (UK) / **on the weekend** (US). Verb government does not transfer: *várok rád* → **I'm waiting for you**; *attól függ* → **it depends on that**; *gratulálok a sikeredhez* → **congratulations on your success**; *köszönöm a segítséget* → **thank you for your help**; *magyarázd el nekem* → **explain it to me** (never *explain me it*); *Péteréknél* → **at Peter's (place)**.

## 6. Names, places, realia

- **Personal names flip to given-name-first**: *Nagy Éva* → **Éva Nagy**; *Petőfi Sándor* → **Sándor Petőfi**. Keep the Hungarian diacritics. Established foreign forms are obligatory: *Liszt Ferenc* → **Franz Liszt**. Historic figures use their English forms: *Kolumbusz Kristóf* → **Christopher Columbus**. Title particles convert and move: *dr. Kovács János* → **Dr. János Kovács**; *ifj. / id. Szabó Péter* → **Péter Szabó Jr. / Sr.**
- **Hungarian exonyms → English exonyms**, never the Hungarian name: *Bécs* → **Vienna**, *Párizs* → **Paris**, *Pozsony* → **Bratislava**, *Bukarest* → **Bucharest**, *Kolozsvár* → **Cluj-Napoca** (add *(Kolozsvár)* in historical/cultural contexts if identity matters).
- **Titles of works**: use the published English title if one exists (*Az ember tragédiája* → **The Tragedy of Man**, *A Pál utcai fiúk* → **The Paul Street Boys**); otherwise translate and give the Hungarian in parentheses on first mention.
- **Realia**: keep + unobtrusive gloss on first mention — *lángos* → **lángos, a deep-fried flatbread**; *érettségi* → **the érettségi, the Hungarian school-leaving exam**; established loans need none (*goulash*, *paprika* — but *paprika* the vegetable is a **pepper**; the spice is **paprika**). Currency: *5 000 Ft* → **HUF 5,000** in business text, **5,000 forints** in prose. *megye* → **county**. Addresses being used as postal addresses stay in Hungarian format.
- Institutions: translate + abbreviate on first mention: *NAV* → **the National Tax and Customs Administration (NAV)**.

## 7. False friends, reversed

The Hungarian word looks international; the English cognate means something else. Translate the meaning:

| Hungarian | trap | correct English |
|---|---|---|
| szimpatikus | sympathetic | **likeable, nice, engaging** |
| aktuális | actual | **current, topical; relevant** |
| akció / akciós | action | **special offer, sale / on sale** |
| korrekt | correct | **fair, decent, professional** |
| kontroll(vizsgálat) | control | **follow-up (exam), check-up** |
| gimnázium | gymnasium | **secondary school, high school** (UK: grammar school) |
| kollégium | college | **dormitory, halls of residence** |
| diploma | diploma | **(university) degree** |
| novella | novel | **short story** |
| regény | — | **novel** |
| recept | receipt | **recipe** (cooking) / **prescription** (medicine) |
| blokk / nyugta | block | **receipt** |
| farmer | farmer | **jeans** |
| szmoking | smoking | **dinner jacket, tuxedo** |
| szolid | solid | **modest, understated** |
| menü (étteremben) | menu | **set meal, daily special** (the card is the *étlap* → **menu**) |
| trafik | traffic | **tobacconist's, newsagent's** |
| kaució | caution | **deposit** |
| konkurencia | concurrence | **competition, competitors** |
| **milliárd** | milliard | **billion** (10⁹) |
| **billió** | billion | **trillion** (10¹²) |

## 8. Formulas, light verbs, particles

- Fixed formulas map to fixed formulas: *Jó étvágyat!* → **Enjoy your meal!** · *Egészségedre!* → **Cheers!** (toast) / **Bless you!** (sneeze) · *Szívesen. / Nincs mit.* → **You're welcome.** · *Jó utat!* → **Have a safe trip!** · *Kéz- és lábtörést!* → **Break a leg!** · *Majd meglátjuk.* → **We'll see.** · *Örvendek.* → **Nice to meet you.** · *Tessék?* → **Sorry? / Pardon?** · *Tessék!* (handing something over) → **Here you are.** · *Megvan!* → **Got it! / Found it!**
- **The treacherous connectives** — each has a lazy dictionary equivalent that is usually wrong:
  - ***pedig*** after a topic = **while/whereas** (plain contrast): *Anna alszik, Péter pedig olvas.* → **Anna is sleeping, while Peter is reading.** Clause-initially = **even though / and yet**: *Pedig mondtam neki.* → **And I did tell him. / Even though I told him.** MT stamps every *pedig* as "however" — almost always wrong.
  - ***illetve*** = **and / or / or rather** by context (*or more precisely* when self-correcting); it means "respectively" only when pairing two lists item-by-item.
  - ***ugyanis*** = **because / as it happens, you see** — never "namely" (that is *nevezetesen/mégpedig*).
  - ***hiába*** — restructure, don't calque "in vain": *Hiába mondtam neki.* → **It was no use telling him. / I told him, but it did no good.**
- Light verbs reversed: *döntést hoz* → **make a decision**; *kérdést tesz fel* → **ask a question**; *fényképet készít* → **take a photo**; *vizsgát tesz* → **take an exam**; *előadást tart* → **give a talk**.
- Discourse particles carry attitude, not lexical meaning — re-express or drop, never calque: *hát* → **well,** · *ugye* → tag question · *azért* → **still / after all** · *ám* → **mind you / though** · *bezzeg* → **but of course** + contrastive stress · *dehogy(is)* → **not at all / of course not** · *hadd* → **let me** (*Hadd segítsek!* → **Let me help!**). Emphatic doubling (*De jó ám!*) → English emphatic *do/really* (**It really is good!**).
- Idioms get English idioms of equal force, or plain language — never word-for-word: *Nem az én asztalom.* → **Not my department.** · *Zsákbamacskát vesz.* → **Buy a pig in a poke.** · *Bagoly mondja verébnek, hogy nagyfejű.* → **The pot calling the kettle black.** · *Vak vezet világtalant.* → **The blind leading the blind.**

## 9. Register without te/ön

The T/V distinction dies in English; compensate with address forms, directness, and contractions — and keep each relationship's level consistent, as the Hungarian did:

- *magázás/önözés* → title + surname (**Mr/Ms Kovács**), no contractions in formal writing, indirect requests: *Kérem, foglaljon helyet.* → **Please have a seat.** · *Meg tudná mondani…?* → **Could you tell me…?** · *Legyen szíves…* → **Would you please…**
- *tegezés* → first names, contractions, direct phrasing: *Figyelj, ezt nézd meg!* → **Hey, look at this!**
- Letters and emails: *Tisztelt Hölgyem/Uram!* → **Dear Sir or Madam,** (US business: **To Whom It May Concern:**) · *Tisztelt Kovács Úr!* → **Dear Mr Kovács,** · *Kedves Anna!* → **Dear Anna,** / informal **Hi Anna,** — the Hungarian **!** after the salutation becomes a **comma** (US business letters: a colon), and the body then starts with a capital.
- Sign-offs: *Üdvözlettel* → **Kind regards / Best regards** · *Tisztelettel* → **Yours sincerely** (named addressee; UK unnamed: **Yours faithfully**) · *Köszönettel* → **Many thanks** · *Puszi/Csók* → **Love,**
- *tetszik*-deference has no English form — plain politeness: *Hogy tetszik lenni?* → **How are you?**

## 10. Punctuation, numbers, formatting

- **Quotes**: „…” and »…« → **"…"** with '…' inside. Fiction **dialogue dashes → quotation marks**, tag order normalized: *– Szia – mondta Péter. – Gyere be!* → **"Hi," said Peter. "Come in!"** Punctuation sits inside the closing quote in US style; UK logical style only if the brief is UK.
- **No comma before *that***: *Azt hiszem, hogy jó.* → **I think (that) it's good.** — the automatic Hungarian comma before *hogy/aki/ami* must NOT surface in English.
- **Relative clauses force a decision Hungarian doesn't mark**: restrictive → no comma (+ *that/who*): *a férfi, aki ott áll* → **the man who is standing there**; non-restrictive → commas + *which/who*: *a ház, amely 1900-ban épült, …* → **the house, which was built in 1900, …** Choose by meaning.
- **Numbers**: decimal comma → **point** (*3,5%* → **3.5%**); space-grouped thousands → **commas** (*1 234,56* → **1,234.56** — informal Hungarian also groups with periods: *5.000 Ft* → **5,000 Ft**, not five); *14.30* → **2:30 p.m.** (or 14:30 in technical/UK text); *fél 8* → **half past seven / 7:30**.
- **Dates ascend**: *2026. június 13.* → **13 June 2026** (UK) / **June 13, 2026** (US); *13-án* → **on the 13th**; *a ’90-es évek* → **the nineties / the 1990s**.
- **Capitalize** months, days, languages, nationalities, holidays, and **I**; headings may take Title Case per the target style guide (sentence case is also fine — be consistent).
- **Dashes**: spaced en-dash asides → **em dashes** (US, unspaced) or spaced en dashes (UK); unspaced range en dash stays (*1995–2005*).
- ***milliárd* → billion, *billió* → trillion** — the reverse of the EN→HU trap, just as catastrophic in finance.

## 11. Hunglish tell list (sweep before returning)

1. Comma before *that* ("I think, that…") — delete.
2. Missing articles (*I am doctor*, *love is the wonderful thing*) — restore *a/an/the*, delete generic *the*.
3. Past simple where present perfect is needed (*I live here since 2020* → **I have lived here since 2020**).
4. Missing do-support, double negatives, missing 3sg *-s* (*he go*).
5. *We were five.* → **There were five of us.** · *According to me* → **In my opinion** · *It depends from* → **it depends on**.
6. *make a photo / make an exam* → **take**; *explain me* → **explain to me**; *Thank you the help* → **thank you for your help**; *I'm agree* → **I agree**.
7. Unflipped names (*Nagy Éva called*), Hungarian date/decimal formats, „low quotes”, spaced dashes.
8. Subject–verb agreement across long subjects; faulty parallelism in lists (*teaching, playing football and a cook* → **…and cooking**); *its/it's*, *your/you're*.
9. Every sentence the same length as its Hungarian source — split the long ones; English breathes shorter.
10. Word-for-word idioms and particles (*bezzeg*, *hát*) still visible — re-express (§8).
11. Register drift: contractions in a formal letter, or stiff formality in banter — re-check the T/V compensation (§9).

## 12. Self-check (HU→EN)

1. Would a native English writer say this, unprompted, in the chosen variety (US/UK)?
2. Information structure re-encoded (cleft/passive/*only*), not copied? Adverbials moved to English positions?
3. Tense chosen by event shape — present perfect where the past touches now, past perfect for earlier-than-past, backshift in reported speech, *used to* vs *usually*?
4. Subjects, dummy *it/there*, objects, articles, possessives, and plurals all restored?
5. Single negation, do-support, correct tags for *ugye*, *whether* for *-e*?
6. Prepositions by English idiom (*in the picture*, *on Monday*, *depends on*, *congratulations on*)?
7. Names flipped, exonyms Englished, realia glossed once, false friends caught (*szimpatikus → likeable*, *milliárd → billion*)?
8. Register compensated consistently — address forms, contractions, salutation comma?
9. English punctuation throughout — no comma before *that*, restrictive vs non-restrictive commas decided, quotes/dates/decimals converted?
10. Filler dropped, idioms idiomatic, sentence rhythm English?
