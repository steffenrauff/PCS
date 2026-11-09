# K21: Benchmark af metadata på programsider – Netflix og Disney+

Kilde: desk research 2026-11-09 af offentlige titelsider (desktop-web, ikke logget ind, da-DK). Besvarer RQ17. Indsigter i [01-eksisterende-indsigter.md](../01-eksisterende-indsigter.md) #44-48.

**Afgrænsning:** Siderne er de offentlige versioner, som Google også viser. Den indloggede app (iOS) og indloggede web kan se anderledes ud. Screenshots mangler. Benchmarket viser markedsstandarden, ikke hvad brugerne forventer.

## Titler
| Tjeneste | Titel | Type | Link |
|---|---|---|---|
| Netflix | Stranger Things | Fiktionsserie | [netflix.com/dk/title/80057281](https://www.netflix.com/dk/title/80057281) |
| Netflix | Love Is Blind | Reality-serie | [netflix.com/dk/title/80996601](https://www.netflix.com/dk/title/80996601) |
| Disney+ | The Simpsons | Animationsserie | [disneyplus.com/da-dk/series/the-simpsons/3ZoBZ52QHb4x](https://www.disneyplus.com/da-dk/series/the-simpsons/3ZoBZ52QHb4x) |
| Disney+ | Family Guy | Animationsserie | [disneyplus.com/da-dk/browse/entity-3c3c0f8b-…](https://www.disneyplus.com/da-dk/browse/entity-3c3c0f8b-7366-4d15-88ab-18050285978e) |

## Sammenligning
| Metadata | TV 2 Play (Forræder UK) | Netflix | Disney+ |
|---|---|---|---|
| **Metadatalinje øverst** | Kanal • genre • antal sæsoner • aldersmærke ("Echo • Reality • 5 sæsoner • Alle") | År • antal sæsoner • alder • **én** genre ("2025 • 5 sæsoner • 16+ • Sci-fi") | År-interval • antal sæsoner • **flere** genrer ("1999 – 2026 • 25 sæsoner • Komedieserie, Animation for voksne, Komedie, Animation") |
| **Genrer** | Én | Én i toppen. 3-4 i "Flere oplysninger" (fx "Dramaserier, Sci-fi-serier, Ungdomsserier og Gyserserier") | 2-4 i toppen og i "Detaljer" |
| **Stemning/tags** | Ingen | Ja: "Denne serie er …" med 8-12 tags, fx "Ildevarslende, Nostalgisk, Uhyggelig" og "Romantisk, Socialt eksperiment, Dating" | Ingen |
| **Medvirkende** | Ikke i metadata | To steder: 2-3 navne lige under beskrivelsen + op til 10 i "Flere oplysninger". Også skabere | I "Detaljer": skaber + 5-6 medvirkende |
| **Produktionsår (serie)** | Nej (kun på film) | Seneste år ("2025", "2026") | Interval ("1989 – 2026") |
| **Antal sæsoner** | Ja | Ja | Ja |
| **Aldersmærke** | Ja | Ja | Ja |
| **Priser/nomineringer** | Ikke set | Som tag ("Golden Globe-nomineret", "Emmy-nomineret") | I den lange beskrivelse |
| **Beskrivelse** | Én tekst med "Læs mere" | Kort (1-2 sætninger) | Kort i toppen + lang i "Detaljer" |
| **Trailere** | Hero-trailer (POC) | Egen sektion med flere trailere/teasere pr. sæson | Ikke set på den offentlige side |
| **Lyd og undertekster** | Ikke tjekket | Ja | Ikon for undertekster |
| **Relateret** | "Andre så også" (set på film) | "Måske vil du også kunne lide" (samme univers først, fx spin-off) | "Du vil måske også synes om" (samme genre/skaber) |

## Observation
1. Begge konkurrenter viser **flere genrer** end Play: Disney+ i toppen, Netflix i en detaljesektion.
2. Kun Netflix viser **stemning/tone** som tags ("Denne serie er …"), og der er mange (8-12).
3. Begge viser **medvirkende** og skaber. Netflix viser 2-3 navne lige under beskrivelsen, så de ses uden at scrolle.
4. Begge viser **år på serier**. Play viser kun år på film.
5. Netflix lægger detaljerne i lag: én genre i toppen, resten længere nede.

## Fortolkning (C)
- Markedsstandarden er flere genrer, medvirkende og år på serier. Play er under standarden på alle tre. Det støtter data stewardens vurdering af "hygiejnefaktor" (#37), men siger ikke noget om, hvad brugerne savner.
- Netflix' stemningstags svarer til feltet "stemning" i Plays nye kategorimodel (K17). Data findes altså allerede hos os.
- Lagdelingen hos Netflix (én genre øverst, flere længere nede) er en mulig model, hvis metadatalinjen ikke skal blive længere.

## Anbefaling
- Afprøv A1 (år), A4 (medvirkende) og A5 (er "Reality" nok?) i sessionerne med spørgsmålet "Hvad mangler du for at vælge?" → RQ0b, RQ4
- Tag screenshots af de indloggede sider (web og iOS) for at bekræfte, at de ligner de offentlige. → RQ17
