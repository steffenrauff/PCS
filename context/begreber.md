# Begreber: "afkode og forstå"

Fælles definition, som al research og tagging bygger på.

**Status:** Udkast. Afstemmes med UX og teamet på en workshop med 3-4 rigtige programsider. Den endelige version logges i [beslutninger.md](beslutninger.md).

## Grundidé
En programside lykkes, når brugeren hurtigt og korrekt kan **beslutte** noget: se nu, gemme, fortsætte eller gå videre. At afkode og forstå er midlet. Beslutningen er målet.

**Definition (PM, workshop 9/11):** At afkode og forstå handler om at **reducere usikkerhed om programmet**. Derfor måles både korrekthed og sikkerhed (se nedenfor).

## Programcyklus: før, under og efter afspilning
Aftalt på workshop med PM 9/11 (K20). Brugerne har forskellige spørgsmål i hver fase.

| Fase | Brugerens spørgsmål (fra workshoppen) | Brugssituationer (afsnit 5) |
|---|---|---|
| Før afspilning | Hvem er med? Hvor mange afsnit? Hvilke aktører er med? | udforske, tjekke-nyt, glaede-sig, lande-direkte |
| Under afspilning | Se videre på programside og forside: hvilke udfordringer er der i dag, og hvad kan optimeres? | fortsaette |
| Efter afspilning | [udfyld: ikke defineret på workshoppen] | |

## Tagging-akser
Hver observation og indsigt tagges på fire akser: **spørgsmål × niveau × årsag × indgang** plus alvorlighed.

### 1. Spørgsmål: hvilken information brugeren leder efter
| Id | Brugerens spørgsmål | Typisk information |
|---|---|---|
| hvad | Hvad er det her? | Type (serie/film/live), genre, format, længde |
| relevans | Er det noget for mig? | Tone, stemning, målgruppe, kvalitetssignaler |
| adgang | Kan jeg se det, og hvordan? | Abonnement, udløb, live/on demand, aldersgrænse |
| navigation | Hvor starter jeg / hvor kom jeg til? | Sæson, episode, fortsæt, rækkefølge |

### 2. Niveau: hvor i forløbet det går galt
| Id | Betydning | Testspørgsmål |
|---|---|---|
| afkode | Kan brugeren finde og aflæse informationen? | Er den synlig, læsbar og til at finde? |
| forstaa | Danner brugeren et korrekt billede af det? | Matcher brugerens forklaring det faktiske indhold? |
| beslutte | Kan brugeren handle på det? | Vælger brugeren uden tøven og korrekt? |

### 3. Årsag: hvor problemet kommer fra
Bruges til at fordele ejerskab ved overdragelsen.

| Id | Betydning | Eksempel |
|---|---|---|
| design | Layout, hierarki, komponent | Udløbsdato står med lille skrift under folden |
| indhold | Tekst, metadata, billeder, redaktionelt | Synopsis er generisk og siger intet om tonen |
| regel | Forretnings- eller rettighedsregel | Indholdet kræver et tilkøb, som ikke forklares |
| ukendt | Kan ikke afgøres ud fra data | |

### 4. Indgang: hvor brugeren kom fra
| Id | Betydning |
|---|---|
| forside | Fra et rail eller en anbefaling |
| soeg | Fra søgning (konkret mål) |
| direkte | Deeplink, push, delt link, ekstern |
| fortsaet | Vender tilbage til noget, de allerede ser |
| ukendt | |

### 5. Brugssituation (udkast, ikke afstemt)
Hvad der skal afkodes og forstås, afhænger af, hvorfor brugeren er på siden. Spejles i Lucid-rammen "Brugssituationer på programsiden".

| Id | Brugerens spørgsmål | Typisk indgang | Kilder (01) |
|---|---|---|---|
| udforske | "Er det her noget for mig?" | Forside, anbefaling, søgning | #1, #17, K16 |
| fortsaette | "Hvor kom jeg til?" | Se videre | #19, #32, K16 |
| tjekke-nyt | "Er der kommet et nyt afsnit? Hvornår kommer det næste?" | Direkte, Min liste | #4, #23, #26 |
| glaede-sig | "Hvornår kommer det, og hvordan bliver jeg mindet om det?" | Kommer snart, trailer, mail | #2, #3, #7, #34 |
| se-live | "Hvornår starter det, og hvad sker der, hvis jeg trykker nu?" | Live-TV, hero | Egne hypoteser |
| lande-direkte | "Hvorfor er jeg her, og hvad kan jeg?" | Mail, SoMe, Google | #8, K11 |

Adgang ("Kan jeg se det, og hvor længe?") går på tværs af alle situationer.

## Matrix: spørgsmål × niveau
Eksempler på, hvad et problem ser ud som i hver celle.

| | afkode | forstaa | beslutte |
|---|---|---|---|
| **hvad** | Kan ikke se, at det er en serie | Tror det er en dokumentar, men det er fiktion | Starter forkert, fordi typen blev misforstået |
| **relevans** | Finder ikke beskrivelsen | Beskrivelsen giver ingen fornemmelse af stemning | Kan ikke afgøre, om det er værd at se |
| **adgang** | Udløb eller pakke er ikke synlig | Forstår ikke, hvad "inkl. i Play Basis" betyder | Vælger at se uden at vide, at det udløber i morgen |
| **navigation** | Finder ikke sæsonvælgeren | Ved ikke, hvilken episode de er kommet til | Starter forfra i stedet for at fortsætte |

## Korrekthed og sikkerhed
Registrér både om brugerens forståelse er **korrekt** og hvor **sikker** brugeren er (lav/middel/høj).
Den mest alvorlige kombination er **forkert + sikker**, fordi brugeren handler på en misforståelse uden at opdage det.

## Sådan observeres hvert niveau
| Niveau | Metode |
|---|---|
| afkode | 5-sekunders-test: "Hvad er det her, og hvad kan du gøre?" |
| forstaa | "Fortæl mig, hvad det handler om, og om det er noget for dig. Hvorfor?" Sammenlign med det faktiske indhold. Spørg ind til sikkerhed. |
| beslutte | En opgave (fx "se næste episode", "find ud af om du kan se den i weekenden"). Observér tøven, fejlvalg og opgivelse. |

## Validering af modellen
Før workshoppen: tag de eksisterende indsigter i [../research/01-eksisterende-indsigter.md](../research/01-eksisterende-indsigter.md) med akserne. Hvis mere end ca. hver femte indsigt ikke passer ind, skal modellen justeres.

## Alvorlighed
| Niveau | Betydning |
|---|---|
| 3 | Brugeren opgiver eller træffer et forkert valg |
| 2 | Brugeren tøver eller må lede, men kommer videre |
| 1 | Mindre irritation eller misforståelse uden konsekvens |

Forkert forståelse med høj sikkerhed er altid mindst 2.

## Afgrænsning
- I scope: programsider for programmer med låst contentID, med fokus på serier. Desktop-web og iOS-app. Se videre på både programside og forside (fasen "under").
- Nedprioriteret: enkeltstående indhold (film, dokumentar).
- Uden for scope: live-events og TV-appen. [Afklar: søgning og afspiller]
