# Duplicate and baseline decisions

## Baseline-princip

Vid första importen behandlas den senaste identifierbara kursplanen som baseline version 1. Äldre versioner som råkar finnas med vid första importen införs inte automatiskt som historiska versioner.

## OMG402

Filer som verkade avse samma kurs:

- `Kurs3_sskgrund_OMG402.pdf`, äldre uppladdad PDF, giltig från 2025-09-01.
- `user_prompt_revision_OMG402_2026-08-31.txt`, reviderad version från användarens prompt, giltig från Hösttermin 2026 (2026-08-31).

Baseline-beslut:

- Vald baseline: `user_prompt_revision_OMG402_2026-08-31.txt`.
- Aktiv kursversion: `OMG402_v01`.
- Exkluderad från aktiv baseline: `Kurs3_sskgrund_OMG402.pdf`.
- Skäl: senare identifierbart giltighetsdatum och uttrycklig användarinstruktion att ersätta tidigare OMG402-information med den reviderade texten.
- Säkerhet: hög.

Den senaste identifierbara OMG402 har behandlats som baseline version 1. Äldre OMG402-fil(er) har inte införts som historiska versioner i datasetet, utan dokumenterats som initiala dubbletter eller äldre upplagor. Framtida ändringar av OMG402 ska versionssättas som OMG402_v02, OMG402_v03 och så vidare.

## Övriga dubbletter

Inga övriga initiala kursplansdubbletter har identifierats i baselinebeslutet. Programplaner och kursplanemall har kopierats som stödmaterial men ingår inte som kursplaner i current-filerna.
