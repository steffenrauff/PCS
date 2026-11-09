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
| **programsiderne** | Serie, enkeltstående program og live-event på desktop-web og iOS | [../context/programsider.md](../context/programsider.md) |

> **Forslag til workshoppen:** "Indholdet" omfatter også adgang (`adgang`). Det er det mest dokumenterede problem i 01, og uden det overser vi den største kendte kilde til forkert forståelse.

## Primært spørgsmål
**Hvor godt hjælper programsiderne brugerne med at afkode og forstå indholdet?**

## Delspørgsmål

### Begrebsafklaring: hvad betyder "afkode" og "forstå"?
Disse spørgsmål kommer først, fordi resten bygger på dem. RQ0a handler om, hvad vi i huset mener. RQ0b handler om, hvad brugerne selv har brug for.

| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ0a | Hvad mener vi i PCS-teamet og på tværs af huset med at **afkode** og **forstå** indholdet på en programside, og hvornår er det lykkedes? | definition | OKR'en bruger ordene uden definition. [begreber.md](../context/begreber.md) er et udkast, og ingen kilde i 01 definerer dem. | Eksisterende viden: workshop, UX-vidensdeling, begrebsområde i Lucid | 1 |
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
| RQ8 | **Hjælper** live-programsiden brugerne med at afkode og forstå, hvornår eventet starter, hvad "Se live kanal" gør før start, og hvordan de bliver påmindet? | `hvad`, `navigation` × alle | Hul 4: ingen brugerdata om live-sider. "Påmind mig" findes kun på iOS. | Ny kvalitativ | 3 |

### Tværgående
| # | Spørgsmål | Dimension | Hvorfor (hul fra 01) | Svares via | Prioritet |
|---|---|---|---|---|---|
| RQ9 | Hvor adskiller afkodning og forståelse sig mellem **desktop-web og iOS**? | platform | Forskellig knaplogik, overlay og påmindelse (#21). | Ny kvalitativ (samme opgaver på begge platforme) | 1 |
| RQ10 | Adskiller problemerne sig efter **indgang** (forside, søgning, direkte link)? | `indgang` | Direkte indgang fra mail skaber forvirring (#8). | Ny kvalitativ (scenarier) + analytics | 3 |

### Eksisterende viden på tværs af huset
De her spørgsmål besvares uden nye sessioner og dækker den del af KR 1, der handler om eksisterende viden.

| # | Spørgsmål | Hvorfor (hul fra 01) | Svares via | Ejer at spørge |
|---|---|---|---|---|
| RQ11 | Hvad viser trailer-A/B-testen om trailerens betydning for engagement og afspilning på programsiden? | Hul 1: der findes et testdesign, men ingen resultater (K12) | Eksisterende | Mette-Sofie Kam |
| RQ12 | Hvor mange kundeservicehenvendelser handler om adgang til konkret indhold, og hvad handler de om? | Hul 6: K09 nævner temaet uden tal | Eksisterende (kundeservice) | [udfyld] |
| RQ13 | Hvordan kommer brugerne ind på programsiderne, og hvor mange afspiller efter et besøg? | Hul 7: tracking findes, men er ikke trukket ud | Analytics | D&I / PDL |
| RQ14 | ~~Hvad viste "Andre så også"-testen?~~ **Besvaret** via Lucid (01 #28-31): genre-match driver relevans. Testen handler om playeren, ikke programsiden. | Hul 3 (K14) | Eksisterende | Steffen Klitlund Rauff |

## Prioritering
0. **Begrebsafklaring:** RQ0a afklares på workshoppen og via UX-vidensdeling i uge 46. RQ0b følger med som åbne spørgsmål i sessionerne.
1. **Adgang og beslutning:** RQ3, RQ5, RQ7, RQ9. Største kendte problem, aldrig testet på selve siden. Kan fungere som baseline for PL-1077.
2. **Afkodning af serie og film:** RQ1, RQ2, RQ4, RQ6. Kernen i objektivet og helt uundersøgt.
3. **Live og indgang:** RQ8, RQ10. Medtages, hvis tiden rækker. Ellers bliver de videnshuller ved overdragelsen.

RQ11-14 sættes i gang med det samme, fordi de ikke kræver rekruttering.

## Sporing: RQ → aktiviteter → indsigter
Opdateres løbende, når der kommer nye kilder eller sessioner. Indsigts-numrene henviser til [01](01-eksisterende-indsigter.md) (evidens i parentes). Spejles i Lucid ("Sporing"-rammen).
*Sidst opdateret: 2026-11-09.*

| RQ | Spørgsmål (kort) | Prio | Aktiviteter | Indsigter indtil nu | Status |
|---|---|---|---|---|---|
| RQ0a | Hvad mener vi med afkode og forstå? | 1 | Workshop m. PM 9/11 · Leah 9/11 · øvrige UX'ere · begrebsområde i Lucid | Ingen kilde definerer ordene. Udkast i begreber.md | Åben |
| RQ0b | Hvad skal brugerne selv forstå for at vælge? | 1 | Design (åbne spørgsmål) · sessioner | #1 skimmer tekst (A) · #17 serie frem for episode (B) · #28 genre driver relevans (B) | Delvist (indirekte) |
| RQ1 | Afkoder de type og handlinger? | 2 | Workshop · design · sessioner | #5 collage-key art forvirrer (B) · #17 (B) | Hul |
| RQ2 | Hvilke elementer afkoder relevans? | 2 | Confluence (titleart, labels) · workshop · sessioner | #1 (A) · #24 "Læs mere" (C) · #27 key art (B) | Delvist |
| RQ3 | Afkoder de adgang, med og uden adgang? | 1 | Confluence (knaplogik) · rekruttering m/u adgang · sessioner | #15 "Sidste chance" forstås (A) · #20 overladt til sig selv (B) · #21 web ≠ app (C) | Hul på selve siden |
| RQ4 | Forstår de hvad det er, og hvor sikre er de? | 2 | Workshop · sessioner | #2 trailers "genreafkoder" (B) · #10 genreord (B) | Hul |
| RQ5 | Forstår de logoer, "kræver X" og udløb? | 1 | Confluence ("Sidste chance") · workshop · sessioner | #11 partnerbrands (B) · #13 live-begreber (A) · #16 én misforståelse (A) · #22 (C) | Delvist (uden for siden) |
| RQ6 | Forstår de, hvor de er i en serie? | 2 | Workshop · sessioner | #4 snigpremiere (B) · #19 nyeste ≠ rigtige (A) · #23 (C) · #26 (C) | Delvist |
| RQ7 | Fører siden til en korrekt beslutning? | 1 | Confluence (hurtig vej til playback) · sessioner | #18 serieindgang (A) · #19 (A) | Hul på selve siden |
| RQ8 | Hjælper live-siden? | 3 | Sessioner (hvis tid) | #3 ønske om påmindelse (B) | Hul |
| RQ9 | Forskel web vs. iOS? | 1 | Rekruttering · sessioner | #21 (C) + egne screenshots | Hul |
| RQ10 | Forskel efter indgang? | 3 | Sessioner (scenarier) · analytics | #8 direkte fra mail (B) · #18 (A) | Delvist |
| RQ11 | Hvad viste trailer-testen? | – | Spørg PM | Testdesign (K12), ingen resultater | Venter |
| RQ12 | Hvad siger kundeservicedata om adgang? | – | Find ejer | #20 nævnt uden tal (B) | Venter |
| RQ13 | Indgang og afspilning efter besøg? | – | D&I / PDL | #31 ASO-klik 1,7K vs. 4,8K (A) | Delvist |
| RQ14 | Hvad viste "Andre så også"? | – | Lucid-board | #28-31 | Besvaret |

## Uden for scope
- Forside, søgning og afspiller, undtagen som indgang til programsiden (RQ10)
- Købsflow og pakkevælger. Upsell overlayet medtages kun, hvor det vises på programsiden.
- TV-app (backlog), Android og mobil-web. Se [../context/beslutninger.md](../context/beslutninger.md).

## Åbne afklaringer
- Er "Kommer snart"-tilstanden (programside før premiere) med? Den er en del af PL-763 og K03, men gør scope bredere.
- Skal deltagerne omfatte både brugere med og uden adgang? Det er en forudsætning for RQ3 og RQ5 og påvirker rekrutteringen.
