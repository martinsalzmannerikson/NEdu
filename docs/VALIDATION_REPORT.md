# Validation report

- Arbetsläge: INITIAL_BUILD av versionshanterat corpus. Tidigare icke-versionerat underlag användes endast som teknisk extraktionsbas.
- Antal relevanta uppladdade originalfiler i manifestet: 44
- Antal filer som kunde läsas eller hanteras: 44
- Antal filer som inte kunde läsas: 0
- Antal kursplaner/kursplansposter identifierade i baseline: 36
- Antal aktiva baseline-kurser: 36
- Antal initiala dubbletter: 1
- Initial dubblett: äldre `Kurs3_sskgrund_OMG402.pdf` har exkluderats från aktiv baseline eftersom reviderad OMG402 med giltighet 2026-08-31 gavs senare i chatten.
- Kursplaner med OCR- eller PDF-läsproblem markerade i notes: 27

## Radantal

- `changes_log.csv`: 37
- `concept_candidates_current.csv`: 67
- `course_content_all_versions.csv`: 559
- `course_content_current.csv`: 559
- `course_sections_all_versions.csv`: 1167
- `course_sections_current.csv`: 1167
- `courses_all_versions.csv`: 36
- `courses_current.csv`: 36
- `evidence_chunks_all_versions.jsonl`: 2560
- `evidence_chunks_current.jsonl`: 2560
- `examinations_all_versions.csv`: 251
- `examinations_current.csv`: 251
- `learning_outcomes_all_versions.csv`: 416
- `learning_outcomes_current.csv`: 416
- `literature_all_versions.csv`: 0
- `literature_current.csv`: 0
- `manifest_files.csv`: 44
- `modules_all_versions.csv`: 168
- `modules_current.csv`: 168

## Kursplaner som saknar lärandemål

- OMG552_v01

## Kursplaner som saknar kursinnehåll

- OMG552_v01

## Kursplaner som saknar examinationsinformation

- OMG552_v01

## Fält som ofta saknas

- revision_date saknas ofta.
- literature saknas i extraherat material.
- semester_or_year_if_stated saknas ofta på kursnivå.
- source_file_hash_if_available saknas för rent saknade kursplaner men finns för kopierade filer och promptkällor.

## Osäkra extraktioner

- OCR-baserade PDF-extraktioner kan ha läsfel, särskilt modulnummer, hp, betyg och vissa kurskoder i PDF-huvuden.
- OMA070 och OMA406 bygger på användarens prompttext eftersom PDF inte fanns som kursplan i uppladdade filer.
- OMG402 bygger på den reviderade prompttexten och är märkt som utkast eftersom beslutsfattare och datum saknas.
- OMG552 saknar kursplan och är endast placeholder.

## Särskild OMG402-notering

Den senaste identifierbara OMG402 har behandlats som baseline version 1. Äldre OMG402-fil(er) har inte införts som historiska versioner i datasetet, utan dokumenterats som initiala dubbletter eller äldre upplagor. Framtida ändringar av OMG402 ska versionssättas som OMG402_v02, OMG402_v03 och så vidare.