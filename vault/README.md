---
type: accueil
tags: [accueil]
---

# Trading KB — vault Obsidian

Ce dossier est la partie « notes » du dépôt `trading-kb`. Tout ce qui est ici se synchronise entre GitHub et Obsidian via le plugin **Obsidian Git**.

## Dossiers

| Dossier | Contenu | Nom de fichier |
|---|---|---|
| `00-Inbox` | Notes rapides à trier | libre |
| `01-Journal` | Une note par jour de trading | `2026-11-03.md` |
| `02-Trades` | Une note par trade | `2026-11-03 ES 1.md` |
| `03-Optionflow` | Relevés GEXBOT 12H / 14H | `Optionflow 2026-11-03.md` |
| `04-Hermes` | Rapports ghost-desk + forward-test | `Hermes 2026-11-03.md` |
| `05-Contexte` | Contexte macro / géopolitique du jour | `Contexte 2026-11-03.md` |
| `06-Orderflow` | Fiches concepts (absorption, POC, CVD…) | nom du concept |
| `Templates` | Modèles à insérer | — |

Les noms datés permettent à la note du journal de lier automatiquement le relevé, le contexte et le rapport Hermes du même jour.

## Routine quotidienne
1. Créer `01-Journal/AAAA-MM-JJ.md` avec le modèle **Journal du jour**.
2. Créer `03-Optionflow/Optionflow AAAA-MM-JJ.md` avec **Releve Optionflow**.
3. Coller le rapport Hermes dans `04-Hermes/Hermes AAAA-MM-JJ.md`.
4. Un fichier par trade dans `02-Trades` avec le modèle **Trade**.

## Suivi forward-test Hermes
```dataview
TABLE hypothese, statut
FROM "vault/04-Hermes"
SORT date DESC
```

## Derniers trades
```dataview
TABLE instrument, sens, resultat_pts, pnl
FROM "vault/02-Trades"
SORT date DESC
LIMIT 20
```
