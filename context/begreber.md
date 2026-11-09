# Begreber: "afkode og forstå"

Fælles definition, som al research og tagging bygger på.

**Status:** Udkast. Afstemmes med UX og teamet på en workshop med 3-4 rigtige programsider. Den endelige version logges i [beslutninger.md](beslutninger.md).

## Grundidé
En programside lykkes, når brugeren hurtigt og korrekt kan **beslutte** noget: se nu, gemme, fortsætte eller gå videre. At afkode og forstå er midlet. Beslutningen er målet.

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
- I scope: [udfyld]
- Uden for scope: [udfyld, fx forside, søgning, afspiller]
