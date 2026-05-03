# Query guide

## Grundprincip

Alla svar ska verifieras mot `text_exact`. Normaliserade fält och begreppskandidater är stöd för sökning, inte självständiga belägg.

## Rekommenderade filer per fråga

| Frågetyp | Primär fil | Kompletterande fil |
|---|---|---|
| Aktuellt kursinnehåll | `data/course_content_current.csv` | `data/evidence_chunks_current.jsonl`, `data/course_sections_current.csv` |
| Lärandemål | `data/learning_outcomes_current.csv` | `data/course_sections_current.csv` |
| Examination | `data/examinations_current.csv` | `data/modules_current.csv` |
| Moduler | `data/modules_current.csv` | `data/examinations_current.csv` |
| Hela kursplaner | `course_markdown/` | `raw_text/` |
| Begrepp | `data/concept_candidates_current.csv` | verifiera i `text_exact` |
| Förändringar över tid | `data/changes_log.csv` | `*_all_versions.*` |
| Tidigare versioner | `data/courses_all_versions.csv` | motsvarande all_versions-filer |

## Rekommenderad svarsmall

Ange alltid:

1. kurskod,
2. kursnamn,
3. program,
4. sektion,
5. exakt textstöd,
6. klassificering: explicit, indirekt/tolkad eller osäker,
7. version om frågan gäller förändring över tid.

## Exempel

Fråga: Vilka kurser innehåller etik?

Arbetssätt: sök i `evidence_chunks_current.jsonl` efter `etik`, `etiska`, `forskningsetik`, `forskaretik`. Bekräfta mot `text_exact`. Klassificera träffen som explicit om ordet förekommer i texten.

Fråga: Var finns VFU?

Arbetssätt: sök efter `VFU`, `verksamhetsförlagd utbildning` och `klinisk utbildning` i `course_sections_current.csv`, `course_content_current.csv` och `examinations_current.csv`.

Fråga: Vad ändrades i OMG402?

Arbetssätt: i detta initiala corpus finns OMG402 endast som baseline v01. Den äldre uppladdade PDF:en är dokumenterad som initial dubblett. Framtida ändringar ska sökas i `changes_log.csv` och `*_all_versions`.
