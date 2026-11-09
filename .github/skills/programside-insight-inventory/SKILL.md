---
name: programside-insight-inventory
description: "Use when collecting, mapping, or summarizing existing knowledge about TV 2 programsider (program pages): reports, MS material, analytics, customer service themes, earlier usability tests, Confluence or PMX canon. Turns sources into rows in research/01-eksisterende-indsigter.md with source, element, dimension, and evidence level. Triggers: eksisterende indsigter, indsigtsoversigt, hvad ved vi allerede, saml viden om programsider."
---

# Indsigtsoversigt for programsider

## Input
- Kilder brugeren giver (filer, links, indsat tekst)
- Shared canon via `pmx-shared-context`: søg på "programside", "program page", "titelside", "PCS"

## Fremgangsmåde
1. Læs [context/begreber.md](../../../context/begreber.md) og [context/programsider.md](../../../context/programsider.md) for akser og element-id'er.
2. Registrér hver ny kilde i tabellen **Kilder** med næste ledige `K##`.
3. Udtræk hver indsigt som én atomar påstand. Én påstand pr. række.
4. Tag med element, spørgsmål (hvad/relevans/adgang/navigation), niveau (afkode/forstaa/beslutte), årsag (design/indhold/regel/ukendt) og evidens (A/B/C).
5. Kan en akse ikke afgøres ud fra kilden, skriv `ukendt`. Passer indsigten slet ikke i modellen, tag `andet`.
6. Spring indsigter uden relevans for afkodning og forståelse over, men nævn dem kort, hvis de er vigtige.
7. Opdatér **Mønstre på tværs** og **Huller i eksisterende viden**.
8. Rapportér andelen af `andet`. Er den over ca. 20 %, så gør opmærksom på, at begrebsmodellen bør justeres.

## Regler
- Citér eller parafrasér tæt. Ingen tal eller citater, der ikke står i kilden.
- Ved modstridende kilder: behold begge rækker og notér konflikten under Mønstre.
- Dato og metode mangler → skriv "ukendt", gæt ikke.

## Output
Opdateret `research/01-eksisterende-indsigter.md` og en kort opsummering: antal kilder, antal indsigter, top-3 mønstre, top-3 huller.
