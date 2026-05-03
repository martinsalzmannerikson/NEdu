# Schema

Saknade värden anges som `missing`. Osäkra tolkningar markeras med `uncertain` eller förklaras i `notes`. Datatyp anges förenklat som text, heltal, decimaltal eller lista.

## manifest_files.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `file_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `original_filename` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `detected_course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `detected_course_name` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `detected_program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `detected_valid_from` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `detected_revision_date` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `file_role` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `included_in_baseline` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `reason_if_excluded` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `matched_course_family_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `matched_course_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `file_hash_if_available` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `readability_status` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## courses_all_versions.csv / courses_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `version_status` | Baseline-, current-, superseded- eller dubblettstatus. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `replaces_course_uid` | Tidigare kursversion som ersätts, annars none. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `superseded_by_course_uid` | Senare kursversion som ersätter denna, annars none. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file_hash_if_available` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_en` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `credits_hp` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `main_field` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `progression` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `cycle` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `semester_or_year_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `syllabus_valid_from` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `decision_date` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `revision_date` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `language` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `department_or_faculty` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `status` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## course_sections_all_versions.csv / course_sections_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `section_unit_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `section` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | learning_outcomes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `original_section_heading` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `subsection` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `unit_type` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `unit_order` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_exact` | Exakt text från kursplanen eller extraherad källa. | text | förklara grundläggande begrepp inom folkhälsa | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_normalized` | Lätt normaliserad text med jämnade radbrytningar. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## learning_outcomes_all_versions.csv / learning_outcomes_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `outcome_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `outcome_order` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `outcome_category_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_exact` | Exakt text från kursplanen eller extraherad källa. | text | förklara grundläggande begrepp inom folkhälsa | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `verb_or_action` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `knowledge_area_candidate` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## course_content_all_versions.csv / course_content_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `content_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `content_order` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_exact` | Exakt text från kursplanen eller extraherad källa. | text | förklara grundläggande begrepp inom folkhälsa | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `content_area_candidate` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `explicit_terms` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## examinations_all_versions.csv / examinations_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `exam_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_code_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_name_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `credits_hp_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `exam_order` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `examination_text_exact` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `examination_category` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `individual_or_group` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `written_or_oral_or_practical_or_clinical` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `mandatory_or_optional` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `grading_scale_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `related_learning_outcomes_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## modules_all_versions.csv / modules_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `module_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_code_if_stated` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_name` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `credits_hp` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_order` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `module_description_exact` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `related_examination_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## literature_all_versions.csv / literature_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `literature_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `author_or_organization` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `year` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `title` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `publication_type` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `mandatory_or_recommended` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_exact` | Exakt text från kursplanen eller extraherad källa. | text | förklara grundläggande begrepp inom folkhälsa | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## evidence_chunks_all_versions.jsonl / evidence_chunks_current.jsonl

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `chunk_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `lineage_confidence` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_uid` | Unik identifierare för en specifik kursversion. | text | OMG402_v01 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_version` | Versionsnummer som heltal. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `is_current` | yes/no om versionen är aktuell. | text | yes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `program` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `education_level` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_code` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_name_sv` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `section` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | learning_outcomes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `text_exact` | Exakt text från kursplanen eller extraherad källa. | text | förklara grundläggande begrepp inom folkhälsa | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `keywords_explicit` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | lista | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `possible_topics` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | lista | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `source_file` | Fil eller promptkälla som texten kommer från. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## concept_candidates_current.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `concept` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `variant_or_exact_phrase` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `frequency` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | heltal | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `appears_in_courses` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `appears_in_sections` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `example_course_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `example_text_exact` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |

## changes_log.csv

| Kolumn | Betydelse | Datatyp | Exempel | Regler för saknade värden |
|---|---|---|---|---|
| `change_id` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `change_date_if_known` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `change_type` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `course_family_id` | Stabil identifierare för kursfamiljen, normalt kurskod. | text | OMG402 | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `old_course_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `new_course_uid` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `section` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | learning_outcomes | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `old_text_exact` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `new_text_exact` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `change_summary` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `change_classification` | Fält enligt filens syfte; se README och QUERY_GUIDE för användning. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `confidence` | Konfidens för extraktion eller klassificering. | text | high | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
| `notes` | Kommentarer, osäkerheter och extraktionsmetod. | text | missing | Skriv `missing`; vid osäkerhet skriv `uncertain` och förklara i `notes`. |
