---
name: programside-session-synthesis
description: "Use when processing usability test or interview notes about TV 2 programsider (program pages). Turns raw session notes in research/sessions/ into tagged observations (element × dimension × severity) and updates research/04-syntese.md. Triggers: sessionsnoter, syntetisér, analysér interview, opdatér syntese, affinity, tagging af observationer."
---

# Sessionssyntese for programsider

## Input
- En eller flere filer i `research/sessions/` (navngivet `P##.md`, se `_skabelon.md`)
- [context/begreber.md](../../../context/begreber.md) for dimensioner og alvorlighed
- [research/01-eksisterende-indsigter.md](../../../research/01-eksisterende-indsigter.md) til sammenligning

## Trin 1: Pr. session
1. Læs de rå noter.
2. Udfyld tabellen **Observationer**: én observeret adfærd eller ét udsagn pr. række.
3. Tag med element, spørgsmål, niveau, årsag og alvorlighed 1–3 (se begreber.md).
4. Udfyld **Korrekt?** og **Sikkerhed**, når noterne gør det muligt. Ellers lades felterne stå tomme. Forkert + høj sikkerhed er mindst alvorlighed 2.
5. Citater skal stå ordret i de rå noter. Ellers lades feltet stå tomt.

## Trin 2: På tværs
1. Gruppér observationer til kerneindsigter. En kerneindsigt kræver mindst 2 deltagere. Ellers markeres den som "enkeltstående".
2. Evidens: A = adfærd hos ≥2 deltagere, B = udsagn eller én deltager, C = fortolkning.
3. Opdatér matricen spørgsmål × niveau og tabellen **Fordeling på årsag** med antal og højeste alvorlighed.
4. Før alle tilfælde af forkert + høj sikkerhed ind i **Forkert + sikker**.
5. Notér forskelle mellem indgange (forside/soeg/direkte/fortsaet), hvis der er data nok. Ellers skriv, at det er et videnshul.
6. Sammenlign med 01: bekræftet, nuanceret eller udfordret.
7. Skriv nye åbne spørgsmål under **Åbne spørgsmål**.

## Regler
- Hold observation, fortolkning og anbefaling adskilt.
- Brug kun pseudonymer (P01 …). Fjern navne og andre persondata, hvis de optræder.
- Overskriv ikke tidligere indsigter. Justér evidens og antal deltagere og notér ændringen.

## Output
Opdaterede sessionsfiler og `research/04-syntese.md` samt en kort opsummering: nye/ændrede kerneindsigter og de mest alvorlige problemer.
