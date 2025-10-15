# Werkwijze met Claude

Dit document beschrijft hoe we samenwerken in deze repository.

## Onderwerpen toevoegen

Wanneer je een nieuw onderwerp hebt voor de presentatie, gebruik dan het volgende formaat:

```
extra onderwerp: [onderwerp beschrijving]
```

Claude zal dit onderwerp dan automatisch toevoegen aan `onderwerpen.md`.

## Logging van antwoorden

Claude schrijft automatisch elk antwoord weg naar een bestand in de `logs/` directory. Elk antwoord krijgt een eigen bestand met een timestamp als bestandsnaam (formaat: `YYYY-MM-DD_HH-MM-SS.md`).

Dit zorgt voor:
- Een overzicht van alle gegeven antwoorden
- Mogelijkheid om terug te kijken naar eerdere antwoorden
- Materiaal voor de presentatie over hoe de conversatie verliep

## Git commits

Bij het maken van commits: geen referentie aan "Generated with Claude" en ook niet "Co-Authored-By: Claude". Gewoon normale commit messages zonder deze referenties.

## Andere commando's

Hier kunnen we in de toekomst meer commando's toevoegen voor andere taken.
