---
name: indsigt-handoff
description: "Use when preparing the handover of the programside insight work to the PCS team before moving to AMP. Builds handoff/videnshuller.md with KR status, prioritized knowledge gaps, suggested methods, and owners. Triggers: overdragelse, handoff, videnshuller, hvad mangler vi at vide, afslut indsigtsarbejde."
---

# Overdragelse af indsigtsgrundlag

## Input
- [research/04-syntese.md](../../../research/04-syntese.md), især Åbne spørgsmål
- [research/01-eksisterende-indsigter.md](../../../research/01-eksisterende-indsigter.md), især Huller
- [context/beslutninger.md](../../../context/beslutninger.md) og [context/stakeholders.md](../../../context/stakeholders.md)

## Fremgangsmåde
1. **Status på KR 1**: hvad er etableret, hvilke dimensioner er godt dækket, og hvor er evidensen svag (kun B/C).
2. **Videnshuller**: saml huller fra 01 og 04, fjern dubletter og formulér hvert hul som et spørgsmål.
3. Prioritér efter (a) betydning for produktbeslutninger og (b) hvor usikker den nuværende viden er.
4. Foreslå en let metode pr. hul (fx analytics-opslag, 5 hurtige tests, survey-spørgsmål).
5. Brug **årsag** (design/indhold/regel) fra syntesen til at foreslå, hvilken funktion hullet hører til. Lad **Ejer** stå tom, medmindre brugeren angiver den.
6. Udfyld **Hvor ligger hvad** og **Kontaktpunkter**.

## Regler
- Teamet skal kunne fortsætte uden at spørge. Undgå interne forkortelser uden forklaring.
- Lov ikke mere, end evidensen bærer.

## Output
Opdateret `handoff/videnshuller.md`. Tilbyd derefter en præsentation via `html-artifacts` eller `pptx` med `tv2-design`.
