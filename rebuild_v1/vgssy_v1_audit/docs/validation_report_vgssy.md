# VGSSY v1 audit validation report
## Scope
This audit covers the Sjuksköterskeprogrammet (VGSSY) education plan and six provided course plans. OMG552 is listed in the education plan but no course plan was provided, so it is marked as missing.
## Source decision for OMG402
The latest uploaded DOCX file for OMG402 is used as the authoritative source in this audit. The older OMG402 PDF is not used for active extraction.
## Counts
- active_course_plans: 6
- education_plans: 1
- programme_courses_listed: 7
- missing_course_plans: 1
- learning_outcomes: 165
- content_items: 221
- modules: 87
- module_alignment_rows: 166
- examination_rows: 124

## Per-course extraction counts

| Course | Learning outcomes | Content items | Modules |
|---|---:|---:|---:|
| MVG201 | 22 | 52 | 17 |
| OMG401 | 27 | 24 | 17 |
| OMG402 | 33 | 32 | 19 |
| OMG403 | 37 | 61 | 18 |
| OMG551 | 33 | 41 | 15 |
| OMG805 | 13 | 11 | 1 |

## Key validation notes
- PDF files for the five included PDF course plans and the education plan had readable text layers with no replacement-character count detected by the extraction script.
- OMG402 was extracted from DOCX. Plain-text DOCX extraction does not preserve visible Word numbering, so learning-outcome order was assigned from list order.
- Module code, module name, hp, grade and linked learning outcomes were extracted into `modules_vgssy.csv`.
- `module_alignment_vgssy.csv` expands module-to-learning-outcome links, including ranges such as 14–20.
- Course literature is not present in the provided source material and is therefore not extracted.
- OMG552 requires a course plan before the programme corpus can be complete.
