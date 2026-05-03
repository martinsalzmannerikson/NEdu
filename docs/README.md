# Kursplanecorpus för vårdvetenskap, omvårdnad och sjuksköterskeutbildning

Detta repo innehåller ett strukturerat, sökbart och versionsförberett kunskapsunderlag baserat på kursplaner inom sjuksköterskeprogram, kompletterande sjuksköterskeutbildning och specialistsjuksköterskeprogram.

## Arbetsläge

Detta paket har byggts som **INITIAL_BUILD** av ett versionshanterat corpus. Ett tidigare icke-versionerat extraktionspaket användes tekniskt som underlag, men inga tidigare historiska versioner har införts. Den första aktiva baseline-versionen för varje kurs är därför `course_version = 1`.

## Baseline och versioner

Varje kurs har:

- `course_family_id`: stabil kursfamilj, normalt kurskod.
- `course_uid`: unik version, till exempel `OMG402_v01`.
- `course_version`: heltal.
- `is_current`: anger om versionen är aktuell.
- `version_status`: anger baseline, current, superseded eller dubbletthantering.

Vid första importen har den senaste identifierbara kursplanen valts som baseline. Äldre initiala dubbletter dokumenteras i `docs/DUPLICATE_AND_BASELINE_DECISIONS.md` och i `data/changes_log.csv`.

## Viktig notering om OMG402

Den senaste identifierbara OMG402, den reviderade versionen med giltighet från Hösttermin 2026 (2026-08-31), har behandlats som baseline version 1: `OMG402_v01`. Den äldre uppladdade OMG402-PDF:en har inte införts som historisk version utan dokumenterats som initial dubblett.

## Filer för sökning

- Aktuellt innehåll: `data/course_content_current.csv`, `data/course_sections_current.csv`, `data/evidence_chunks_current.jsonl`.
- Lärandemål: `data/learning_outcomes_current.csv`.
- Examination: `data/examinations_current.csv`.
- Moduler: `data/modules_current.csv`.
- Hela kursplaner: `course_markdown/` och `raw_text/`.
- Begrepp: `data/concept_candidates_current.csv`, alltid verifierat mot `text_exact`.
- Historik och framtida ändringar: `*_all_versions.*` och `data/changes_log.csv`.

## Svar med textstöd

Framtida svar bör alltid ange kurskod, kursnamn, program, sektion, exakt textstöd och om träffen är explicit, indirekt eller osäker. Vid versionsfrågor ska även `course_uid` och `course_version` anges.

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

