# Livrables & implémentation — la règle anti-PDF-mort

Le risque de ce parcours : produire de beaux documents qui finissent oubliés sur un Drive.
On l'évite avec une règle simple : **tout livrable = 3 briques**. Un module n'est terminé
que quand les 3 sont posées.

## Les 3 briques de tout livrable

1. **Outil vivant** — le document est éditable et fait pour être MODIFIÉ (pas un PDF figé) :
   un doc partagé, un tableur, un dashboard, une page de manuel. On peut le changer quand la
   réalité change.
2. **Rituel** — un moment récurrent où on le REVOIT, posé dans l'agenda ou en tâche planifiée
   (sinon il meurt). Ex : revue trimestrielle du cap, revue mensuelle du goulot, mise à jour
   d'un SOP à chaque incident.
3. **Lieu** — un endroit unique où il VIT et se consulte par toute l'équipe : l'espace Circle
   de la boîte, un Notion, le manuel de la boîte. Pas « quelque part dans mes fichiers ».

Coach Zaki ne clôt pas un module tant qu'il n'a pas fait nommer au membre : *quel outil,
quel rituel (quand), quel lieu.*

## Outils concrets par module (préférer le gratuit ; cf. flag dépendances plugin)

| Module | Livrable | Outil vivant | Rituel | Lieu |
|---|---|---|---|---|
| 1 · Vision/Mission/Valeurs | Doc « âme » + valeurs traduites en comportements | Doc éditable (Google Doc / Notion) | Relecture à **chaque intégration** + revue annuelle | Épinglé dans l'espace de la boîte |
| 2 · Plan stratégique | Objectifs 9 sphères × horizons | Doc/tableur, priorités du trimestre visibles | **Revue trimestrielle** + revue mensuelle (agenda) | Plan affiché, espace de la boîte |
| 3 · Diagnostic | Arbre de contrainte + carte process priorisée | Tableur (1 ligne/fonction, statut goulot) | **Revue mensuelle** : « c'est quoi LE goulot ce mois ? » | Même tableur partagé équipe |
| 4 · SOP | 1-3 SOP + manuel | Manuel de la boîte (Notion / Circle / Skool interne) | **Rituel boîte noire** : à chaque incident, on amende le SOP écrit | Le manuel = la source unique |
| 5 · Outils & données | Audit + **CRM** + conventions de comptage | Tableur/CRM avec « prochaine action » | **Créneau hebdo** de mise à jour et de relance | Un seul endroit, accès équipe |
| 6 · Équipe | Organigramme + fiches de rôle + pipeline | Fiches « scorecard » (résultats attendus) + tracker candidats (même logique que le CRM) | Revue des rôles à chaque recrutement/départ | Manuel / espace RH |
| 7 · Délégation & rythme | Dashboard KPI + cadence + QC | **Dashboard** (tableur ou page HTML) alimenté par le CRM + checklists QC | **Cadence** : quotidien / hebdo / individuels / mensuel / trimestriel (événements agenda) | Dashboard partagé + agenda équipe |

## Déploiement des outils (à l'export) — ce qu'on peut vraiment brancher

L'export (`ctp-export`) ne fait pas que compiler : il **déploie** la couche outils avec ce qui
est connecté au Claude du membre. Toujours **proposer et confirmer** avant de créer quoi que ce
soit d'externe.

- **Cadence de réunions** → créer les **événements récurrents** dans l'agenda du membre
  (MCP calendar) : daily huddle, hebdo équipe, revue mensuelle du goulot, revue trimestrielle du cap.
- **Dashboard KPI** → générer un **tableur** prérempli (colonnes = les KPI choisis au module 5)
  ou une **page HTML** de dashboard autonome, à alimenter.
- **Rituels de contrôle qualité** → une **tâche planifiée locale** (scheduled-tasks) qui rappelle
  la revue QC + le passage des checklists.
- **Manuel de la boîte** → structure de départ (arborescence des SOP) prête à coller dans
  Notion / l'espace Circle de la boîte.
- **Le cap** → épinglé en tête de l'espace Circle de la boîte, visible par l'équipe.

Principe : chaque livrable sort du parcours **branché à un déclencheur réel** (un événement
d'agenda, une tâche planifiée, une page consultée en équipe), jamais en simple fichier.

## Garde-fous outils
- **Toujours une voie gratuite** (tableur, doc, agenda) ; les outils payants restent optionnels
  avec disclaimer coût. (cf. flag dépendances plugin CTP.)
- Ne créer un événement / une tâche / un fichier externe **qu'après accord** du membre.
- Le membre doit pouvoir tout tenir **sans dépendre d'un prestataire à vie**.
