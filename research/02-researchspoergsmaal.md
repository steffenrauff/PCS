# Researchspørgsmål

**Status:** Udkast 2026-11-07. Afstemmes på workshoppen sammen med [../context/begreber.md](../context/begreber.md).

## Forankring i OKR
- **Objective:** *"Gøre det lettere for brugerne at afkode og forstå indholdet på programsiderne."*
- **KR 1:** *"…et fælles indsigtsgrundlag for, hvor godt programsiderne hjælper brugerne med at afkode og forstå indholdet, baseret på eksisterende viden på tværs af huset og nye kvalitative indsigter."*

Spørgsmålene bruger OKR'ens egne ord og læses sådan:
| OKR-ord | Betydning i researchen | Akse i begreber.md |
|---|---|---|
| **afkode** | Kan brugeren finde og aflæse informationen på siden? | niveau `afkode` |
| **forstå** | Danner brugeren et korrekt billede, og hvor sikker er brugeren? | niveau `forstaa` + korrekthed/sikkerhed |
| **hjælper** | Fører afkodning og forståelse til en sikker og korrekt beslutning (se, gem, gå videre)? | niveau `beslutte` |
| **indholdet** | Hvad det er, om det er noget for mig, om og hvordan jeg kan se det, og hvor jeg starter | spørgsmål `hvad`, `relevans`, `adgang`, `navigation` |
| **programsiderne** | Serier med låst contentID på desktop-web og iOS. Live-events er uden for scope, og enkeltstående indhold er nedprioriteret (beslutning 9/11) | [../context/programsider.md](../context/programsider.md) |
| **(ramme)** | Programcyklus: før, under og efter afspilning (beslutning 9/11) | fase i [begreber.md](../context/begreber.md) |

> **Forslag til workshoppen:** "Indholdet" omfatter også adgang (`adgang`). Det er det mest dokumenterede problem i 01, og uden det overser vi den største kendte kilde til forkert forståelse.

## Overordnede spørgsmål
KR 1 bygger på "eksisterende viden på tværs af huset og nye kvalitative indsigter". Derfor er der to spor med hvert sit overordnede spørgsmål:

| Spor | Overordnet spørgsmål | Delspørgsmål | Kilder |
|---|---|---|---|
| **HS1: Internt** | **Hvad ved vi, og hvad antager vi, internt om brugernes behov for at afkode og forstå programsiderne?** | RQ0a, RQ11, RQ15-17 | Indsigtsoversigt (01), workshop, UX-vidensdeling, data |
| **HS2: Brugerne** | **Hvor godt hjælper programsiderne brugerne med at afkode og forstå indholdet?** | RQ0b, RQ1-10 | Nye kvalitative sessioner |

I HS1 skelnes der mellem det, vi **ved** (evidens A/B), og det, vi **antager** (evidens C, fx workshop-antagelser og egne screenshot-hypoteser). HS2 afprøver de vigtigste antagelser fra HS1. Det er derfor, workshoppen kommer før sessionerne.

## Delspørgsmål

### Begrebsafklaring: hvad betyder "afkode" og "forstå"?
Disse spørgsmål kommer først, fordi resten bygger på dem. RQ0a handler om, hvad vi i huset mener. RQ0b handler om, hvad brugerne selv har brug for.

| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ0a | Hvad mener vi i PCS-teamet og på tværs af huset med at **afkode** og **forstå** indholdet på en programside, og hvornår er det lykkedes? **Besvaret 9/11:** at reducere usikkerhed om programmet (K20). **Afkode** – brugeren kan finde og aflæse informationen på siden. **Forstå** – brugeren danner et korrekt billede af det, hun har aflæst, og ved, hvor sikker hun er. PM og UX er enige i definitionen i begreber.md. | definition | OKR'en bruger ordene uden definition. [begreber.md](../context/begreber.md) er et udkast, og ingen kilde i 01 definerer dem. | Eksisterende viden: workshop, UX-vidensdeling, begrebsområde i Lucid | 1 |
| RQ0b | Hvilken information har brugerne selv brug for at afkode og forstå på en programside for at kunne træffe et valg, og hvornår oplever de, at de har "forstået nok"? | definition × `beslutte` | Vi ved, at brugerne skimmer tekst (#1), orienterer sig efter serien (#17) og vurderer relevans ud fra genre (#28). Men vi ved ikke, hvad brugerne selv regner for at have forstået en side. | Ny kvalitativ (åbne spørgsmål før opgaverne) + eksisterende viden | 1 |

### Afkode
| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ1 | Kan brugerne på få sekunder **afkode**, hvilket indhold programsiden præsenterer (serie, film eller live), og hvad de kan gøre? | `hvad` × `afkode` | Hul 5: den almindelige programside er ikke testet. Key art er vigtig for afkodning (#5, #17). | Ny kvalitativ | 2 |
| RQ2 | Hvilke elementer bruger brugerne til at **afkode**, om indholdet er noget for dem (key art, beskrivelse, genre, labels), og finder de dem? | `relevans` × `afkode` | Brugerne skimmer tekst for at beslutte (#1). Afkortning med "Læs mere" (#24) og key art (#27) påvirker afkodningen. | Ny kvalitativ | 2 |
| RQ3 | Kan brugerne **afkode**, om og hvor længe de kan se indholdet, både med og uden adgang? | `adgang` × `afkode` | Hul 2: ingen test af adgang på selve programsiden (#20). Web og iOS kommunikerer adgang forskelligt (#21). | Ny kvalitativ | 1 |

### Forstå
| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ4 | **Forstår** brugerne korrekt, hvad indholdet er og handler om (type, genre, tone), og hvor sikre er de? | `hvad`, `relevans` × `forstaa` | Kun indirekte viden: trailers hjælper med at "genreafkode" (#2), og genreord påvirker interessen (#10). | Ny kvalitativ | 2 |
| RQ5 | **Forstår** brugerne, hvad kanal- og partnerlogoer, "kræver X" og udløbslabels betyder for, om de kan se indholdet? | `adgang` × `forstaa` | Brugerne er i tvivl om partnerbrands (#11) og live-begreber (#13). Udløbslabels misforstås i enkelte tilfælde (#16, #22). | Ny kvalitativ | 1 |
| RQ6 | **Forstår** brugerne, hvor de er i en serie, og hvad "Afspil S#:E#", sæsonvælger og labels som "Tilføjet i går" fortæller dem? | `navigation` × `forstaa` | Tvivl om, hvad der er "nyt" (#4). "Tilføjet i går" vs. "Ny episode" (#23). Episodeantal mangler (#26). Hypotese: "5 sæsoner" men Sæson 2-6. | Ny kvalitativ | 2 |

### Hjælper (beslutte)
| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ7 | **Hjælper** programsiden brugerne til at beslutte (se nu, gem eller gå videre) uden tøven og korrekt? Hvor tøver de, vælger forkert eller opgiver? | alle × `beslutte` | Serieindgang giver bedst adfærd på forsiden (#18), men selve programsiden er ikke undersøgt. Den nyeste episode er ikke altid den rigtige (#19). | Ny kvalitativ | 1 |
| RQ8 | ~~**Hjælper** live-programsiden brugerne med at afkode og forstå, hvornår eventet starter, hvad "Se live kanal" gør før start, og hvordan de bliver påmindet?~~ **Uden for scope** (beslutning 9/11). Bliver et videnshul. | `hvad`, `navigation` × alle | Hul 4: ingen brugerdata om live-sider. "Påmind mig" findes kun på iOS. | Ny kvalitativ | 3 |

### Tværgående
| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ9 | Hvor adskiller afkodning og forståelse sig mellem **desktop-web og iOS**? | platform | Forskellig knaplogik, overlay og påmindelse (#21). | Ny kvalitativ (samme opgaver på begge platforme) | 1 |
| RQ10 | Adskiller problemerne sig efter **indgang** (forside, søgning, direkte link)? | `indgang` | Direkte indgang fra mail skaber forvirring (#8). | Ny kvalitativ (scenarier) + analytics | 3 |
| RQ18 | Hvilke udfordringer har brugerne med **Se videre** på programsiden og forsiden i dag, og hvor er der optimeringspunkter? | `navigation` × alle, fase "under" | PM's fokus for fasen "under afspilning" (K20). Den nyeste episode er ikke altid den rigtige (#19), og næste episode opleves som "underlig" (#32). | Ny kvalitativ + analytics | 2 |

### Eksisterende viden på tværs af huset
De her spørgsmål besvares uden nye sessioner og dækker den del af KR 1, der handler om eksisterende viden.

| # | Spørgsmål | Hvorfor (hul fra 01) | Svares via | Ejer at spørge |
|---|---|---|---|---|
| RQ15 | Hvad **antager** PCS-teamet om, hvor godt brugerne kan afkode og forstå programsiderne, og hvilke af antagelserne er vi mest usikre på? **Besvaret 9/11:** fem antagelser fra PM (01 A1-A5). | Teamets viden er ikke dokumenteret nogen steder. Eneste antagelser indtil nu er mine egne screenshot-hypoteser (C) i [programsider.md](../context/programsider.md). | Workshop "Hvad tror vi, brugerne forstår?" (antagelser + 2×2: vigtig × sikker) | PCS-teamet / Mette-Sofie Kam |
| RQ16 | Hvad **ved** vi fra tidligere undersøgelser om brugernes oplevelse af programsiden i forhold til deres evne til at afkode og forstå indholdet? **Besvaret 9/11.** | Kun få fund handler om selve programsiden (hul 5). UX'ernes viden er ikke samlet ét sted. | UX-vidensdeling (Leah, Marie-Louise, Jakob, øvrige), URR, Lucid-boards | UX'erne |
| RQ11 | Hvilke indsigter har vi om **trailerens betydning for brugerens valg om at afspille** indhold fra programsiden? **Delvist besvaret** (K19, 01 #38-43): ingen entydig effekt på tværs, positivt signal på store skærme (TV), intet signal på mobil, og få ser traileren. Mangler: desktop-web, iOS og tidlige stop. | Hul 1: der fandtes et testdesign, men ingen resultater (K12). Nu delvist dækket af POC-slides (K19). | Eksisterende (trailer-POC, PL-763) | Mette-Sofie Kam |
| RQ17 | **Benchmark:** Hvordan udstiller andre tjenester metadata på deres programsider, fx flere genrer eller stemninger som bullets og medvirkende, og hvad er markedsstandarden, som brugerne kan have med sig? | Data steward vurderer, at mere metadata og medvirkende er en hygiejnefaktor (01 #37, C). Play viser i dag én genre. | Benchmark (desk research): Netflix (nævnt i K18) og Disney+. Viser markedsstandarden, ikke brugernes forventning. | skra |

## Prioritering
0. **Begrebsafklaring og antagelser:** RQ0a og RQ15 afklares på workshoppen og via UX-vidensdeling i uge 46. RQ15's 2×2 (vigtig + usikker) bruges til at prioritere RQ1-10 før design. RQ0b følger med som åbne spørgsmål i sessionerne.
1. **Adgang og beslutning:** RQ3, RQ5, RQ7, RQ9. Største kendte problem, aldrig testet på selve siden. Kan fungere som baseline for PL-1077.
2. **Afkodning af serie og film:** RQ1, RQ2, RQ4, RQ6. Kernen i objektivet og helt uundersøgt.
3. **Live og indgang:** RQ8, RQ10. Medtages, hvis tiden rækker. Ellers bliver de videnshuller ved overdragelsen.

RQ11 og RQ15-17 sættes i gang med det samme, fordi de ikke kræver rekruttering.

## Sporing: RQ → aktiviteter → indsigter
Opdateres løbende, når der kommer nye kilder eller sessioner. Indsigts-numrene henviser til [01](01-eksisterende-indsigter.md) (evidens i parentes). Spejles i Lucid ("Sporing"-rammen).
*Sidst opdateret: 2026-11-12.*

| Spor | RQ | Spørgsmål (kort) | Prio | Aktiviteter | Indsigter indtil nu | Status |
|---|---|---|---|---|---|---|
| **HS1** | | **Internt: Hvad ved vi, og hvad antager vi, internt om brugernes behov for at afkode og forstå programsiderne?** | | | | |
| HS1 | RQ0a | Hvad mener vi med afkode og forstå? | 1 | • Workshop m. PM 9/11<br>• Leah 9/11<br>• øvrige UX'ere<br>• begrebsområde i Lucid | **Workshop 9/11 (K20, C):** At afkode og forstå er at **reducere usikkerhed om programmet**, så vi måler både korrekthed og sikkerhed.<br>**Afkode** – brugeren kan finde og aflæse informationen på siden: Er den synlig, læsbar og til at finde?<br>**Forstå** – brugeren danner et korrekt billede af det, hun har aflæst, og ved, hvor sikker hun er.<br>Rammeværk: før, under og efter afspilning. "Under" = Se videre på programside og forside (RQ18). "Efter" er ikke defineret. PM og UX er enige i definitionen i begreber.md | Besvaret |
| HS1 | RQ15 | Hvad antager teamet om, hvor godt brugerne afkoder og forstår, og hvor er vi mest usikre? | 1 | • Workshop "Hvad tror vi, brugerne forstår?" 9/11<br>• 2×2-prioritering | **Workshop 9/11 (K20, C):** Fem antagelser fra PM, alle om metadata i fasen *før*: A1 produktionsår på serier · A2 antal afsnit (#26) · A3 overblik over alle Forræder-produktioner (#33, #35) · A4 medvirkende (#37) · A5 er "Reality" nok, eller skal der mere kategorisering til (#10, #28, #36). Plus 11 screenshot-hypoteser (C) i programsider.md | Besvaret |
| HS1 | RQ16 | Hvad ved vi fra tidligere undersøgelser om brugernes evne til at afkode og forstå programsiden? | 1 | • Leah 9/11<br>• Marie-Louise og Jakob (svaret)<br>• øvrige UX'ere<br>• URR og Lucid-boards | #1, #2, #4 (K02) · #7-9 (K03) · #32 næste episode (C) · #33-35 Indholdsrelationer (C)<br>**Fortolkning: indholdsrelationer (C)**<br>**Afkode:** Brugeren kan kun aflæse det, der står på siden. Ligger sæsoner, trailere, bonusmateriale og resten af en franchise ikke dér, ser brugeren ikke, at det findes (#33-35).<br>**Forstå:** Relationerne giver kontekst, fx "del 2", "ny sæson på vej" eller "samme univers". Genre og univers er det, brugerne vurderer relevans ud fra (#28).<br>**Beslutte:** Siden skal støtte både at udforske og at fortsætte. Uden relationer mister brugeren overblikket over næste skridt.<br>**Årsag:** regel (PEI), ikke design. | Besvaret |
| HS1 | RQ11 | Hvilke indsigter er der om trailerens betydning for valget om at afspille? | 1 | • Trailer-POC-slides (K19)<br>• Spørg PM om desktop-web, iOS og tidlige stop | **Trailer-POC (K19):**<br>• Ingen entydig effekt på aktivering: 3 af 41 delanalyser signifikante, to højere og én lavere (#38, A)<br>• Store skærme: 6 af 8 titler har højere aktivering med trailer på Android TV eller Smart TV, ikke signifikanstestet (#39, A)<br>• Få ser traileren: 5-11 % ser mindst halvdelen på desktop og TV, ca. 2 % på Android mobil (#40, A)<br>• Mobil: intet positivt signal, flere søgninger og lavere aktivering (#41, A)<br>• Før premiere finder brugerne programsiden via Google ca. 2 uger før, men trailervideoen i søgeresultatet giver næsten ingen klik (#42-43, A)<br>**Fortolkning (C):** Traileren er ikke en generel løftestang for afspilning. Den kan afstemme forventninger på store skærme, men få ser den, så key art og tekst bærer stadig afkodningen. | Delvist |
| HS1 | RQ17 | Benchmark: hvordan udstiller andre tjenester metadata på programsider? | 2 | • Benchmark af Netflix og Disney+ (K21)<br>• Screenshots af indloggede sider (web, iOS) | #37 mere metadata er hygiejne (C) · **K21 (C):** Begge viser flere genrer (#44), medvirkende (#46) og år på serier (#47). Kun Netflix viser stemningstags (#45) og lægger detaljer i lag (#48). Play er under standarden på genrer, medvirkende og år | Delvist |
| **HS2** | | **Brugerne: Hvor godt hjælper programsiderne brugerne med at afkode og forstå indholdet?** | | | | |
| HS2 | RQ0b | Hvad skal brugerne selv forstå for at vælge? | 1 | • Design (åbne spørgsmål)<br>• sessioner | #1 skimmer tekst (A) · #17 serie frem for episode (B) · #28 genre driver relevans (B) · #49-50 medvirkende kan påvirke valg (B, selvrapporteret og ikke specifikt på programsiden) | Delvist (indirekte) |
| HS2 | RQ1 | Afkoder de type og handlinger? | 2 | • Workshop<br>• design<br>• sessioner | #5 collage-key art forvirrer (B) · #17 (B) | Hul |
| HS2 | RQ2 | Hvilke elementer afkoder relevans? | 2 | • Confluence (titleart, labels)<br>• workshop<br>• sessioner | #1 (A) · #24 "Læs mere" (C) · #27 key art (B) | Delvist |
| HS2 | RQ3 | Afkoder de adgang, med og uden adgang? | 1 | • Confluence (knaplogik)<br>• rekruttering m/u adgang<br>• sessioner | #15 "Sidste chance" forstås (A) · #20 overladt til sig selv (B) · #21 web ≠ app (C) | Hul på selve siden |
| HS2 | RQ4 | Forstår de hvad det er, og hvor sikre er de? | 2 | • Workshop<br>• sessioner | #2 trailers "genreafkoder" (B) · #10 genreord (B) | Hul |
| HS2 | RQ5 | Forstår de logoer, "kræver X" og udløb? | 1 | • Confluence ("Sidste chance")<br>• workshop<br>• sessioner | #11 partnerbrands (B) · #13 live-begreber (A) · #16 én misforståelse (A) · #22 (C) | Delvist (uden for siden) |
| HS2 | RQ6 | Forstår de, hvor de er i en serie? | 2 | • Workshop<br>• sessioner | #4 snigpremiere (B) · #19 nyeste ≠ rigtige (A) · #23 (C) · #26 (C) · #32 næste episode "underlig" (C) | Delvist |
| HS2 | RQ7 | Fører siden til en korrekt beslutning? | 1 | • Confluence (hurtig vej til playback)<br>• sessioner | #18 serieindgang (A) · #19 (A) · #32 (C) | Hul på selve siden |
| HS2 | RQ8 | Hjælper live-siden? | 3 | Sessioner (hvis tid) | #3 ønske om påmindelse (B) | Hul |
| HS2 | RQ9 | Forskel web vs. iOS? | 1 | • Rekruttering<br>• sessioner | #21 (C) + egne screenshots | Hul |
| HS2 | RQ10 | Forskel efter indgang? | 3 | • Sessioner (scenarier)<br>• analytics | #8 direkte fra mail (B) · #18 (A) | Delvist |

## Uden for scope
- Forside, søgning og afspiller, undtagen som indgang til programsiden (RQ10)
- Købsflow og pakkevælger. Upsell overlayet medtages kun, hvor det vises på programsiden.
- TV-app (backlog), Android og mobil-web. Se [../context/beslutninger.md](../context/beslutninger.md).

## Åbne afklaringer
- Er "Kommer snart"-tilstanden (programside før premiere) med? Den er en del af PL-763 og K03, men gør scope bredere.
- Skal deltagerne omfatte både brugere med og uden adgang? Det er en forudsætning for RQ3 og RQ5 og påvirker rekrutteringen.
