# PCS – Indsigtsgrundlag for programsider (C4 2026)

## Formål
Workspacet understøtter KR 1 i [okr.md](okr.md): et fælles indsigtsgrundlag for, hvor godt programsiderne hjælper brugerne med at afkode og forstå indholdet. Arbejdet overdrages til teamet 30. nov.

## Sprog og stil
- Skriv på dansk. Kort, konkret, uden konsulentsprog.
- Adskil altid **observation** (hvad skete), **fortolkning** (hvad betyder det) og **anbefaling**.

## Evidensregler
- Hver indsigt skal have kilde (fil, link eller session-id) og evidensniveau:
  - **A**: Observeret adfærd hos flere brugere (test, analytics)
  - **B**: Selvrapporteret eller enkeltstående observation (interview, survey, kundeservice)
  - **C**: Antagelse, intern vurdering eller ekspertudsagn
- Opfind aldrig citater, tal eller kilder. Mangler der data, skriv det som et videnshul.
- Tag efter akserne i [context/begreber.md](context/begreber.md) (spørgsmål × niveau × årsag × indgang + alvorlighed) og elementnavnene i [context/programsider.md](context/programsider.md).

## Struktur
- `context/`: stabil viden (programsider, begreber, stakeholders, beslutninger)
- `research/`: researchforløbet i rækkefølge 01 → 04, plus `sessions/`
- `handoff/`: overdragelse til teamet
- `.github/skills/`: workflows for indsigtsoversigt, sessionssyntese og overdragelse

## Workflow
1. Søg først eksisterende viden via `pmx-shared-context`, før du skriver nyt.
2. Log beslutninger om scope og metode i [context/beslutninger.md](context/beslutninger.md).
3. Opdatér [research/04-syntese.md](research/04-syntese.md) efter hver sessionsrunde, ikke kun til sidst.
