# Known limitations

- Flera PDF-filer krävde OCR eller föregående OCR-baserad extraktion. Detta kan ha påverkat kurskoder i sidhuvuden, radbrytningar, modulnummer, hp och betyg.
- Kurslitteratur har inte kunnat extraheras som litteraturlista. `literature_*` finns därför som tomma schemafiler.
- OMG402 är en reviderad promptversion och saknar fastställd beslutsfattare och beslutsdatum i texten.
- OMA070 och OMA406 bygger på användarens inskrivna kursplanetext snarare än uppladdad PDF.
- Begreppskandidaterna är ett empiriskt register över faktiska fraser, inte en komplett teoretisk kodbok.
- Semantiska frågor ska alltid verifieras mot `text_exact` innan de används akademiskt eller administrativt.
- Jämförelser över tid fungerar först fullt ut när framtida revideringar läggs in som v02, v03 osv. Den äldre initiala OMG402-PDF:en är inte införd som historisk version enligt baseline-regeln.
