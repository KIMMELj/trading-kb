---
type: journal
date: {{date:YYYY-MM-DD}}
tags: [journal]
---

# {{date:dddd DD MMMM YYYY}}

## Contexte
- Macro / news : [[Contexte {{date:YYYY-MM-DD}}]]
- Option flow : [[Optionflow {{date:YYYY-MM-DD}}]]
- Rapport Hermes : [[Hermes {{date:YYYY-MM-DD}}]]

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
