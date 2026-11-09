# K19: Trailer POC (PL-763) – samlet overblik

Kilde: slides om trailer-POC'en, delt 2026-11-09. Ejer og link: ukendt. Opfølgning på testdesignet i K12. Indsigter i [01-eksisterende-indsigter.md](../01-eksisterende-indsigter.md) #38-43.

> Samlet visuelt i frame "Trailer POC: hvad ved vi? (K19)" på [workshop-boardet i Lucid](https://lucid.app/lucidspark/62e18d5d-2302-4878-98dd-a89c367b0710/edit).

## Testen i korte træk
| | Før premiere | Efter premiere |
|---|---|---|
| Spørgsmål | Kan traileren give tidligt engagement (set trailer, Min liste, aktivering fra "mere som dette") og synlighed i Google? | Giver trailer på programsiden højere aktivering end kontrol uden trailer? |
| Metode | Google-data for 9 titler | 50/50 A/B-test, 41 delanalyser (titel, platform, periode, treatment) |

## Efter premiere: aktivering
| Screenshot | Opsummering |
|---|---|
| ![Trailer POC efter premiere](../../context/screenshots/trailer-poc-efter-premiere.png) | **Observation**<br>• Ingen entydig effekt på tværs: 3 af 41 delanalyser er signifikante, to højere og én lavere (#38).<br>• Store skærme: 6 af 8 titler har højere aktivering med trailer på Android TV eller Smart TV efter trailerstart ved 0 sek. Android TV: 5/1/2 (højere/uændret/lavere). Smart TV: 2/5/1. Ikke signifikanstestet (#39).<br>• Få ser traileren: 5-11 % ser mindst halvdelen på desktop og TV, max 18 % (Hvem byder bedst, desktop). Android mobil: ca. 2 % halvdelen, ca. 1 % hele (#40).<br>• Mobil: intet positivt signal. Flere søgninger, lavere aktivering (#41).<br><br>**Fortolkning (C)**<br>• På store skærme kan traileren afstemme forventningen til indholdet, før brugeren trykker afspil. Data viser kun aktivering, ikke hvorfor.<br>• POC'ens arbejdshypotese: mobil bruges til at søge og orientere sig, og afspilningen sker på en anden skærm. |

## Før premiere: synlighed i Google
| Screenshot | Opsummering |
|---|---|
| ![Trailer POC Google før premiere](../../context/screenshots/trailer-poc-google-foer-premiere.png) | **Observation**<br>• Søgning på titlen begynder i gennemsnit 13 dage før premiere (6-22), omkring traileren. For 5 af 9 titler lidt før (#42).<br>• 10.298 klik fra Google før premiere på 9 titler (27.218 visninger). Alle 9 havde flest klik på premieredagen.<br>• POC'ens anbefaling: Programsiden skal være live og kunne findes i Google, før traileren lanceres, og gerne 2-3 uger før premiere.<br>• 100 knive fik knap halvdelen af alle klik før premiere på tværs af de 9 titler. 34 % af 100 knives egne klik kom før premiere (søgbar i 22 dage), mod 13-24 % for de øvrige (søgbare i 6-18 dage).<br>• Korpset: søgninger startede 18/8, to dage før traileren (20/8). 241 klik og 6 videoklik før premiere (5.092 visninger).<br><br>**Fortolkning (C)**<br>• Længere søgbarhed ser ud til at give flere klik, men det er en sammenhæng, ikke en årsag. Det støtter K10's pointe om, at infohint 4 uger før premiere er for sent (#25). |
| ![Nybyggerne klik fra Google](../../context/screenshots/trailer-poc-nybyggerne.png) | **Observation**<br>• Nybyggerne: søgestigning fra 2/9, trailer live 7/9, premiere og flest klik 14/9 (154 klik).<br>• Før premiere: 240 klik, 1.860 visninger, **0 videoklik** (#43).<br>• Sæsonen kører stadig, og klikkene topper igen ugentligt efter premiere.<br><br>**Fortolkning (C)**<br>• Brugerne finder programsiden via Google, men trailervideoen i søgeresultatet giver næsten ingen klik. |

## Konsolideret
1. **Traileren er ikke en generel løftestang.** Effekten er positiv på store skærme, neutral på tværs og fraværende på mobil.
2. **Signalet ligger uden for vores scope.** TV er i backlog. Mobil (nærmest iOS) viser intet signal. Der er ikke noget separat resultat for desktop-web.
3. **Få ser traileren.** Selv på desktop og TV ser højst ca. hver tiende mindst halvdelen. Traileren kan ikke bære afkodningen alene. Key art og tekst er stadig de vigtigste kilder (#1, #17).
4. **Programsiden er en indgang før premiere.** Brugerne søger ca. to uger før, og jo længere siden er søgbar, jo flere klik.

## Anbefaling
- Test Jacobs proxy på POC-data: Stopper trailergruppen færre afspilninger tidligt end kontrolgruppen (K18, videnshul #3)? → RQ11, RQ13
- Bed om et separat resultat for desktop-web og iOS og om signifikanstest af de nye Adobe-tal. → RQ11
- I sessionerne: Spørg, hvad brugeren forventer, før og efter traileren. → RQ2, RQ4
