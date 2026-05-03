# Update guide

## Lägga in en ny kursplan

1. Identifiera kurskod, kursnamn, program, giltighetsdatum och beslutsdatum.
2. Om kurskoden inte finns i `courses_all_versions.csv`, skapa ny `course_family_id` och `course_uid` med suffix `_v01`.
3. Lägg till rader i all_versions-filerna.
4. Markera `is_current = yes`.
5. Lägg till `new_course_added` i `changes_log.csv`.
6. Återskapa current-filerna från all_versions-filerna.

## Reviderad kursplan

1. Matcha mot befintlig `course_family_id`.
2. Bestäm nästa versionsnummer, exempelvis `OMG402_v02`.
3. Sätt tidigare version till `is_current = no` och `superseded_by_course_uid = ny version`.
4. Sätt ny version till `is_current = yes` och `replaces_course_uid = tidigare version`.
5. Jämför metadata, lärandemål, innehåll, examinationer och moduler.
6. Skriv konkreta ändringar i `changes_log.csv`.
7. Behåll samtliga historiska rader i all_versions-filerna.
8. Återskapa current-filerna så att de endast innehåller aktuell version.

## Dubbletter

Om två filer verkar avse samma kurs och samma version, skapa inte ny version. Dokumentera i `manifest_files.csv` och `docs/DUPLICATE_AND_BASELINE_DECISIONS.md`.

## Kurskod ändras

Om kurskod ändras men kursen verkar motsvara samma kursfamilj, markera `course_family_id`-matchningen som `uncertain`, dokumentera skäl i `notes` och skapa ändringstyp `metadata_changed` eller `uncertain_change` i `changes_log.csv`.

## OMG402

Den aktuella baseline är `OMG402_v01`. Nästa revidering ska bli `OMG402_v02`, inte en ny baseline.
