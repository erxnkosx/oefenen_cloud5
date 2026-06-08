# Oefening 2 — GitHub Actions: regels code tellen en als artifact uploaden

Je krijgt een klein script. Je hoeft de code niet aan te passen.

## Gevraagd
Schrijf een workflow die bij elke push:
1. het aantal regels code van `app.js` telt en wegschrijft naar een tijdelijke file.
   In Bash doe je dat met:  `wc -l app.js > /tmp/linesofcode.txt`
2. die tijdelijke file uploadt als **artifact** met de naam `linesofcode`.

## Tips
- Tellen = een gewoon shell-commando -> gebruik een `run:`-stap.
- Uploaden = een bestaande action -> gebruik `actions/upload-artifact` met `name` en `path`.
- Vergeet `actions/checkout` niet als eerste stap.
- Controleer in het tabblad Actions dat de run groen is en het artifact downloadbaar is.

Zet je oplossing in een mapje `vraag-github-actions`.
