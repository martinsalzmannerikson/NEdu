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

- `changes_log.csv`: 38
- `concept_candidates_current.csv`: 67
- `course_content_all_versions.csv`: 580
- `course_content_current.csv`: 580
- `course_sections_all_versions.csv`: 1218
- `course_sections_current.csv`: 1218
- `courses_all_versions.csv`: 36
- `courses_current.csv`: 36
- `evidence_chunks_all_versions.jsonl`: 2611
- `evidence_chunks_current.jsonl`: 2611
- `examinations_all_versions.csv`: 260
- `examinations_current.csv`: 260
- `learning_outcomes_all_versions.csv`: 430
- `learning_outcomes_current.csv`: 430
- `literature_all_versions.csv`: 0
- `literature_current.csv`: 0
- `manifest_files.csv`: 44
- `modules_all_versions.csv`: 173
- `modules_current.csv`: 173

## Kursplaner som saknar lärandemål

- Inga identifierade efter OMG552-uppdateringen.

## Kursplaner som saknar kursinnehåll

- Inga identifierade efter OMG552-uppdateringen.

## Kursplaner som saknar examinationsinformation

- Inga identifierade efter OMG552-uppdateringen.

## Fält som ofta saknas

- revision_date saknas ofta.
- literature saknas i extraherat material.
- semester_or_year_if_stated saknas ofta på kursnivå.
- decision_date saknas för OMG552 eftersom datum inte anges i den bifogade kursplanen.

## Osäkra extraktioner

- OCR-baserade PDF-extraktioner kan ha läsfel, särskilt modulnummer, hp, betyg och vissa kurskoder i PDF-huvuden.
- OMA070 och OMA406 bygger på användarens prompttext eftersom PDF inte fanns som kursplan i uppladdade filer.
- OMG402 bygger på den reviderade prompttexten och är märkt som utkast eftersom beslutsfattare och datum saknas.
- OMG552 bygger på uppladdad DOCX med valbar text; beslutsdatum och revisionsdatum saknas i källtexten.

## Särskild OMG402-notering

Den senaste identifierbara OMG402 har behandlats som baseline version 1. Äldre OMG402-fil(er) har inte införts som historiska versioner i datasetet, utan dokumenterats som initiala dubbletter eller äldre upplagor. Framtida ändringar av OMG402 ska versionssättas som OMG402_v02, OMG402_v03 och så vidare.
