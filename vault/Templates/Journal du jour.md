---
type: journal
date: {{date:YYYY-MM-DD}}
tags: [journal]
---

# {{date:dddd DD MMMM YYYY}}

## Contexte
- Macro / news : [[vault/05-Contexte/Contexte {{date:YYYY-MM-DD}}|Contexte {{date:YYYY-MM-DD}}]]
- Option flow : [[vault/03-Optionflow/Optionflow {{date:YYYY-MM-DD}}|Optionflow {{date:YYYY-MM-DD}}]]
- Rapport Hermes : [[vault/04-Hermes/Hermes {{date:YYYY-MM-DD}}|Hermes {{date:YYYY-MM-DD}}]]

## Scénario du jour
- Régime attendu :
- Niveaux à surveiller :
- Invalidation :

## Trades
```dataview
TABLE instrument, sens, resultat_pts, pnl
FROM "vault/02-Trades"
WHERE date = this.date
```

## Debrief
- Ce qui a marché :
- Ce qui n'a pas marché :
- À retenir :
