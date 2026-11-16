# Serier: behov og brugerrejser

Status: researchkladde, ikke researchfund. Dokumenteret 2026-11-16.

Hører til: [undersøgelsesdesign](03-undersoegelsesdesign.md) og [beslutninger](../context/beslutninger.md).

## Preely og kildegrundlag

- Kilder: brugerens afklaringer og godkendelser i samtalen "Preely survey om serier", dokumenteret 2026-11-16, samt den oprettede og gennemgåede Preely-kladde. Originalkilderne er ikke offentligt tilgængelige.
- Denne offentlige version er godkendt til PCS uden Preely-link, workspace-navn eller interne projekt-, test-, spørgsmåls- og sessions-id'er.
- Ved afslutning af opsætningen var både deltagerlink og paneldeling deaktiveret. Intet var sendt ud, og Preely viste 0 deltagere. Tekniske gennemløb foregik i preview, ikke som researchbesvarelser.
- Denne fil dokumenterer opsætningen, men synkroniseres ikke automatisk med Preely.
- Platformreference: [Preelys vejledning om branching](https://preely.com/academy/branching/).

## Formål og afgrænsning

Undersøge, hvilke behov brugerne har i deres rejser omkring serier, og hvordan programsiden hjælper eller hindrer dem i at komme videre.

Serier er første anvendelsesområde for et rammeværk, der senere kan afprøves på andre indholdstyper. Undersøgelsen skal ikke kortlægge programsidens samlede anvendelse.

Dette er et andet undersøgelsesdesign end det tidligere [billedbaserede surveyscript](survey-script.md). Det tidligere script bevares. Denne kladde dokumenterer brugerens valgte retning for Preely-surveyet, ikke en ny PM/UX-godkendelse af det samlede PCS-scope.

- Arbejdsafgrænsningen omfatter fiktionsserier, dokumentarserier og realityserier.
- Film, sport, live og nyheder er udenfor.
- Enheden for analysen er ét konkret serierelateret besøg inden for den seneste uge.
- Rejser både med og uden programsiden indgår. Ved flere programsider bruges den senest besøgte.
- Der vises ikke et screenshot i denne version. Det tidligere billede af *Spillet* var materiale til et andet, billedbaseret undersøgelsesdesign.
- Tidligere fiktive interviewfund er illustrative hypoteser, ikke evidens. De er ikke gemt som fund her.

## Rammeværk, version 1

| Dimension | Det skal undersøgelsen belyse |
|---|---|
| Anledning og kontekst | Hvad satte besøget i gang, og hvilken enhed blev brugt? |
| Mål | Hvad ville brugeren opnå før mødet med programsiden? |
| Behov | Hvad skulle brugeren vide, afklare eller kunne gøre? |
| Forløb | Hvad skete før, på og efter siden? Indgik siden overhovedet? |
| Sidens bidrag | Hvad hjalp siden med, og hvad blev ikke løst eller løst andre steder? |
| Resultat og konsekvens | Lykkedes brugeren, og hvad gjorde vedkommende ved eventuelle mangler? |

Det genbrugelige er strukturen. Behovskategorier fra serier er ikke på forhånd valideret for andre indholdstyper.

## Faktisk Preely-opsætning

- Sprog: dansk.
- Almindelige spørgsmål: `Open-ended question` eller `Multiple choice` med ét svar.
- Screening: separate godkendelsesregler pr. svar.
- Forgrening: `Branching` med to svarknapper og spring frem eller afslutning.
- Demografiske standardspørgsmål: deaktiveret.
- Ingen respondentbilleder eller klikopgaver.
- De følgende afvigelser fra det oprindelige udkast blev godkendt af brugeren:
  - Spørgsmålet om programsidebesøg har "Ja" og "Nej / usikker". Et efterfølgende spørgsmål adskiller nej og usikker på den relevante vej.
  - Det sidste spørgsmål er delt i "Manglede du noget?" og et fælles fritekstfelt for "Ja / i tvivl". "Nej" afslutter.
- Spørgsmålet om samlet resultat og spørgsmålet om mangler findes i hver sin kopi på de to veje. Deltageren ser kun én kopi af hvert spørgsmål.

### Rækkefølge og routing

Numrene er interne labels i Preely, ikke et krav om synlige spørgsmålsnumre for deltagerne.

| Label | Type | Næste trin |
|---|---|---|
| 01 Screening - seneste besøg | Screening, ét svar | Første tre svar → 02. Øvrige → screeningafslutning |
| 02 Besøgets mål | Åbent | 03 |
| 03 Primært formål | Ét svar | 04 |
| 04 Anledning | Åbent | 05 |
| 05 Enhed | Ét svar | 06 |
| 06 Programside besøgt | Branching | Ja → 07. Nej / usikker → 06B |
| 07 Titel og vej ind | Åbent | 08 |
| 08 Behov på siden | Åbent | 09 |
| 09 Brug af siden | Åbent | 10 |
| 10 Sidens hjælp | Ét svar | 11 |
| 11 Næste handling | Ét svar | 12A |
| 12A Resultat - med side | Ét svar | 13A |
| 13A Mangler - med side | Branching | Ja / i tvivl → 14. Nej → tak og afslutning |
| 06B Nej eller usikker | Ét svar | Begge svar → 07B |
| 07B Rejse uden sikker side | Åbent | 12B |
| 12B Resultat - uden side | Ét svar | 13B |
| 13B Mangler - uden side | Branching | Ja / i tvivl → 14. Nej → tak og afslutning |
| 14 Uddyb mangler | Åbent | Tak og afslutning |

13A springer over hele B-forløbet. Deltagere med et bekræftet programsidebesøg får derfor ikke spørgsmålene til dem uden eller med usikkert besøg.

## Tekst i surveyet

### Velkomst

Titel: **Sidste gang du brugte TV 2 Play i forbindelse med en serie**

> Vi vil gerne forstå, hvad du har brug for, når du bruger TV 2 Play i forbindelse med serier.
>
> Tænk på den seneste gang, du ville finde, undersøge eller se en serie. Det er lige så relevant, hvis du ikke endte med at se noget.
>
> Her tæller både fiktionsserier, dokumentarserier og realityserier med. Besvar spørgsmålene ud fra det konkrete besøg, ikke hvad du normalt gør.

### 01 Screening - seneste besøg

**Hvornår brugte du senest TV 2 Play i forbindelse med en serie?**

- I dag
- I går
- For 2-7 dage siden
- For mere end 7 dage siden
- Det har jeg ikke gjort
- Det husker jeg ikke

De første tre svar har politikken `Approved`. De sidste tre har `End flow`.

Screeningafslutning:

> Tak for din interesse. Denne undersøgelse handler om oplevelser fra den seneste uge, så du behøver ikke besvare flere spørgsmål.

### 02 Besøgets mål

**Hvad ville du gerne ved det besøg?**

Beskriv kort med dine egne ord. Skriv gerne seriens navn, hvis det handlede om en bestemt serie.

### 03 Primært formål

**Hvad beskriver bedst dit vigtigste formål ved besøget?**

- Finde en serie uden at have en bestemt i tankerne
- Vurdere, om en bestemt serie var noget for mig
- Begynde på en serie, jeg allerede havde besluttet at se
- Fortsætte eller genoptage en serie
- Finde et bestemt afsnit eller en bestemt sæson
- Tjekke, om der var kommet nye afsnit, eller hvornår de kom
- Finde eller gemme en serie til senere
- Noget andet
- Husker ikke

### 04 Anledning

**Hvad fik dig til at åbne TV 2 Play ved netop det besøg?**

Beskriv kort, hvad der satte besøget i gang.

### 05 Enhed

**Hvilken enhed brugte du ved besøget?**

- TV
- Mobil
- Tablet
- Computer
- Anden enhed
- Flere enheder
- Husker ikke

### 06 Programside besøgt

**Åbnede du under besøget en side for en bestemt serie?**

Vi mener siden med information om serien og eksempelvis sæsoner, afsnit og en afspilningsknap. Ikke forsiden eller selve videoafspilleren.

- Ja → 07
- Nej / usikker → 06B

### 07 Titel og vej ind

**Hvilken serie var siden for, og hvordan kom du ind på den?**

Hvis du åbnede flere seriesider under besøget, skal de næste spørgsmål handle om den sidste, du åbnede.

Skriv gerne, hvad du gjorde lige inden. Hvis du ikke husker seriens navn, kan du beskrive den.

### 08 Behov på siden

**Hvad ville du finde ud af eller gøre, da du kom ind på siden?**

Hvis du ikke havde et bestemt formål med at åbne siden, må du gerne skrive det.

### 09 Brug af siden

**Hvad brugte du på siden?**

Beskriv de informationer eller muligheder, du brugte, og hvad du brugte dem til. Skriv gerne “intet”, hvis du blot gik videre.

### 10 Sidens hjælp

**I hvilken grad hjalp siden dig med det, du ville?**

- Slet ikke
- I mindre grad
- I nogen grad
- I høj grad
- Fuldt ud
- Jeg havde ikke et bestemt mål på siden
- Ved ikke

### 11 Næste handling

**Hvad gjorde du umiddelbart efter siden?**

- Startede eller fortsatte afspilning
- Gik videre til andet indhold i TV 2 Play
- Søgte efter information uden for TV 2 Play
- Forlod TV 2 Play
- Noget andet
- Husker ikke

### 06B Nej eller usikker

**Du svarede “Nej / usikker”. Hvilket svar beskriver bedst dit besøg?**

- Jeg besøgte ikke en side for en bestemt serie
- Jeg er usikker / husker ikke, om jeg besøgte en side for en bestemt serie

### 07B Rejse uden sikker side

**Hvordan gik du frem for at gøre det, du ville?**

Beskriv kort, hvad du gjorde fra starten af besøget, til du stoppede eller begyndte at se noget.

### 12A / 12B Samlet resultat

Samme ordlyd i de to Preely-elementer:

**Fik du ved besøget gjort det, du oprindeligt ville?**

- Ja
- Delvist
- Nej
- Mit formål ændrede sig undervejs
- Ved ikke

### 13A / 13B Mangler

Samme ordlyd i de to Preely-elementer:

**Var der noget, du manglede at vide eller kunne gøre undervejs?**

Hvis du er i tvivl, kan du vælge “Ja / i tvivl” og beskrive det på næste side.

- Ja / i tvivl → 14
- Nej → tak og afslutning

### 14 Uddyb mangler

**Hvad manglede du at vide eller kunne gøre undervejs?**

Beskriv gerne, hvad det var, og hvad du gjorde som følge af det. Hvis du er i tvivl, må du gerne beskrive din usikkerhed.

### Tak og afslutning

Samme tekst ved normal afslutning og ved "Nej" i 13A/13B:

> Tak for din hjælp. Dine svar hjælper os med at forstå, hvad brugerne har brug for i forskellige situationer omkring serier.

## Analyse og begrænsninger

- Kod hvert besøg efter rammeværkets seks dimensioner. Brug konkrete svar som belæg; udfyld ikke manglende oplysninger med antagelser.
- Hold åbne beskrivelser af mål adskilt fra de efterfølgende hjulpne kategorier.
- Sammenhold 08, 09, 10 og 14 for programsidebesøg. En høj vurdering alene dokumenterer ikke, at siden er kritisk.
- Saml 12A/12B som samme analysemål, men bevar markeringen af vej. Gør tilsvarende for 13A/13B. Manglende svar fra den anden vej er strukturelt fravalg, ikke frafald.
- Adskil "besøgte ikke" fra "usikker / husker ikke". Usikkerhed er ikke evidens for, at siden blev sprunget over.
- Et besøg uden afspilning kan være vellykket, eksempelvis ved et afklaret fravalg eller en afklaret udgivelsesdato.
- Materialet er selvrapportering. Det kan pege på bidrag og barrierer, men beviser ikke nødvendighed eller årsagssammenhænge.
- Kommende surveybesvarelser har evidensniveau **B** efter PCS' model. Denne kladde indeholder endnu ingen observationer eller fund. Fortolkninger og anbefalinger skal holdes adskilt fra besvarelserne.
- Resultater gælder de undersøgte serierelaterede besøg og rekrutteringen, ikke alle brugere eller alle indholdstyper. Repræsentativitet er ikke etableret.

## Før udsendelse

- Afstem med PM og UX, hvordan denne retning indgår i det samlede PCS-forløb. Surveyet spørger til besøg på alle enheder; det ændrer ikke i sig selv det tidligere platformsvalg for de observerede tests.
- Pilotér spørgeforståelse, læsbarhed, længde og de foreløbige svarkategorier med målgruppen. Teknisk preview erstatter ikke en respondentpilot.
- Rekruttér også uden for programsiden, så rejser uden siden kan indgå.
- Fastlæg rekruttering og ønsket bredde mellem serietyper, enheder og besøgsformål.
- Åbn ikke deling eller udsend invitationer uden en særskilt beslutning.
- Ved senere ændringer i Preely skal denne fil og routingtabellen opdateres eksplicit.
