# Programsider

## Hvad er en programside
Den side på TV 2 Play, der præsenterer ét stykke indhold: en serie, et enkeltstående program eller et live-event. Brugeren skal her afgøre, hvad indholdet er, om det er noget for dem, og hvordan de kommer i gang.

Platforme: desktop-web og iOS-app er bekræftet og i scope (se [beslutninger.md](beslutninger.md)). På iOS åbner programsiden som et ark med luk (X) og cast-knap. TV-app: i backlog. Mobil-web og Android: [udfyld]

### Forskelle desktop-web vs. iOS-app
| Element | Desktop-web | iOS-app |
|---|---|---|
| `hero` | Keyart til højre, tekst til venstre | Keyart øverst i fuld bredde, tekst under |
| `cta` vs. `beskrivelse` | Synopsis over Afspil | Afspil over synopsis |
| `beskrivelse` | Ca. 2 linjer | Ca. 3 linjer, mere af præmissen synlig |
| Sekundære handlinger | "Min liste" som knap | "Del" og "Min liste" som ikoner |
| Live: påmindelse | Mangler | "Påmind mig" under "Se live kanal" |
| Live: nedtælling | Lille, ved CTA | Stor, midt i hero |

## Varianter
| Variant | Eksempel | Særlige elementer |
|---|---|---|
| Serie | Forræder UK (reality, 5 sæsoner) | Sæsonvælger, episodeliste, "Afspil S#:E#" |
| Enkeltstående program (film, dokumentar) | Sweet Home Alabama (film, 2002) | Ingen sæsoner. Varighed og år i metadata. "Afspil" uden episode. Rail "Andre så også". |
| Live-event (fx fodboldkamp) | Serie A: Roma-Sassuolo (Sport X, i aften 20.40) | Metadata over titlen, nedtælling, "Se live kanal". Web: ingen sekundær handling. iOS: "Påmind mig". Rail "Se med live" med status ("Live 17.45-20.25", "I morgen 12.25") og fremdriftslinje. |

## Elementer
Brug disse navne konsekvent i tagging.

| Element-id | Element | Beskrivelse |
|---|---|---|
| hero | Hero / topbillede | Stort keyart i højre side, der fader ud mod venstre |
| titel | Titel | Serie og film: logografik. Live: almindelig tekst ("Serie A: Roma-Sassuolo") |
| beskrivelse | Beskrivelse / synopsis | Ca. 2 linjer, afkortet med "Læs mere". Live: én linje, der gentager titlen. |
| metadata | Kanal/brand, genre, år, varighed, antal sæsoner, aldersmærkning | Én linje. Serie: "[Echo-logo] Echo • Reality • 5 sæsoner • [Alle]". Film: "[TV 2-logo] • Romantik • 1 t. 44 min • 2002 • [Alle]". Live: "[logo] Sport X • [I aften] 20.40 • Fodbold", placeret over titlen. |
| label | Statusmærke | Gul mærkat, fx "Tilføjet i går" (film) eller "I aften" (live) |
| tilgaengelighed | Udløbsdato, abonnement, live/on demand | Udløb og abonnement ses ikke i hero på nogen af eksemplerne. Live: nedtælling til start (timer/min/sek). |
| cta | Afspil / fortsæt / min liste | Serie: "Afspil S2:E1". Film: "Afspil". Begge med "Min liste" (iOS også "Del"). Live: rød "Se live kanal". iOS har desuden "Påmind mig". |
| saesoner | Sæson- og episodevælger | Chips pr. sæson ("Sæson 2" … "Sæson 6") med episoderække under |
| relateret | Relateret indhold | Film: rail "Andre så også", hvor flere kort har C MORE-logo. Live: rail "Se med live". |

## Screenshots
[Læg i `context/screenshots/` og link her]
- Serie, web: [Forræder UK](screenshots/serie-forraeder-uk-web.png) (2026-11-07)
- Film, web: [Sweet Home Alabama](screenshots/film-sweet-home-alabama-web.png) (2026-11-07)
- Live, web: [Serie A: Roma-Sassuolo](screenshots/live-roma-sassuolo-web.png) (2026-11-07)
- Serie, iOS: [Forræder UK](screenshots/serie-forraeder-uk-ios.png) (2026-11-07)
- Film, iOS: [Sweet Home Alabama](screenshots/film-sweet-home-alabama-ios.png) (2026-11-07)
- Live, iOS: [Serie A: Roma-Sassuolo](screenshots/live-roma-sassuolo-ios.png) (2026-11-07)

## Kendte problemer og hypoteser
| Hypotese | Kilde | Evidens (A/B/C) |
|---|---|---|
| Metadata siger "5 sæsoner", men vælgeren viser Sæson 2-6. Brugeren kan blive i tvivl om, hvor serien starter, og om sæson 1 mangler (`navigation` × `forstaa`, `metadata`/`saesoner`). | Screenshots Forræder UK, web og iOS, 2026-11-07 | C |
| Synopsen afkortes, før præmissen er forklaret ("…det ultimative spil om…"). Brugeren skal klikke "Læs mere" for at vurdere relevans (`relevans` × `afkode`, `beskrivelse`). Mindre udtalt på iOS. | Screenshots Forræder UK, web og iOS, 2026-11-07 | C |
| Kanal/brand-logoet ("Echo") siger ikke nødvendigvis brugeren noget om adgang eller indholdstype (`hvad`/`adgang` × `forstaa`, `metadata`). | Screenshot Forræder UK, web, 2026-11-07 | C |
| Udløb og abonnementskrav vises ikke i hero (`adgang` × `afkode`, `tilgaengelighed`). **Nuanceret:** Screenshots er taget som bruger med adgang. Udløb vises som label tæt på udløb, og "kræver X" vises for brugere uden adgang (01 #15, K10). | Screenshots af alle tre varianter, web og iOS, 2026-11-07 | C |
| Siden viser, hvornår indholdet kom ("Tilføjet i går"), men ikke hvornår det forsvinder. Nyhed er synlig, udløb er ikke (`adgang` × `afkode`, `label`/`tilgaengelighed`). | Screenshot Sweet Home Alabama, web, 2026-11-07 | C |
| Kanal/brand-logoet skifter mellem programsider (Echo, TV 2, C MORE i relateret). Brugeren kan ikke afgøre, om logoet betyder noget for adgang (`adgang` × `forstaa`, `metadata`/`relateret`). **Støttet:** Brugere er i tvivl om, hvad SkyShowtime, BritBox og C More betyder (01 #11, B). | Screenshots Forræder UK og Sweet Home Alabama, web, 2026-11-07 | C |
| C MORE-mærket indhold anbefales i "Andre så også" uden tegn på, om brugerens abonnement dækker det (`adgang` × `beslutte`, `relateret`). Hænger sammen med PL-1077. | Screenshot Sweet Home Alabama, web, 2026-11-07 | C |
| "Se live kanal" vises ca. 50 min før kampstart. Det er uklart, om knappen viser kampen eller det, der kører på Sport X nu (`hvad` × `beslutte`, `cta`). | Screenshots Roma-Sassuolo, web og iOS, 2026-11-07 | C |
| Live-siden på desktop-web har ingen påmindelse, men det har iOS ("Påmind mig"). Web-brugere, der ikke kan se nu, har ingen handling (`navigation` × `beslutte`, `cta`). Jf. påmindelse i PL-763. | Screenshots Roma-Sassuolo, web og iOS, 2026-11-07 | C |
| Live-beskrivelsen gentager titlen og giver ingen grund til at se (betydning, stilling, kommentator) (`relevans` × `forstaa`, `beskrivelse`, årsag `indhold`). | Screenshot Roma-Sassuolo, web, 2026-11-07 | C |
| Det fremgår ikke, om Sport X kræver en bestemt pakke (`adgang` × `afkode`, `metadata`/`tilgaengelighed`). | Screenshot Roma-Sassuolo, web, 2026-11-07 | C |
