# Template — `process/<slug>/STATE.md`

Créer ce fichier au **premier lancement** du parcours pour un projet, puis le mettre à jour **à la
fin de chaque module** (c'est lui que `ctp-process` lit pour afficher la carte et recommander la
prochaine étape). Copier le bloc ci-dessous tel quel et le remplir au fil de l'eau.

---

```markdown
# PARCOURS PROCESS — projet « <slug> »

> Démarré le : <date> · Dernière mise à jour : <date>
> Coach Zaki : <actif | sur demande>  (réglé dans `ctp/coach-mode.md`)

## Carte d'avancement
| # | Étape | Statut | Livrable | Où il vit | Quand on le revoit |
|---|-------|--------|----------|-----------|--------------------|
| 0 | Gate | ⬜ | GO / pas encore | — | — |
| 1 | Vision, Mission, Valeurs | ⬜ | `ame-vision-mission-valeurs.md` | | |
| 2 | Plan stratégique | ⬜ | `plan-strategique.md` | | |
| 3 | Diagnostic-goulot | ⬜ | `diagnostic-goulot.md` + `carte-process.md` | | |
| 4 | SOP | ⬜ | `sop/` + `manuel.md` | | |
| 5 | Outils & données (CRM) | ⬜ | `audit-outils.md` + `crm.md` + `conventions-donnees.md` | | |
| 6 | Équipe | ⬜ | `organigramme.md` + `fiches-role.md` + `pipeline-recrutement.md` | | |
| 7 | Délégation & rythme | ⬜ | `dashboard-kpi.md` + `cadence.md` + `qc.md` | | |
| 8 | Export & implémentation | ⬜ | `REFERENCE.md` | | |

Légende : ✅ complet (checklist entièrement cochée) · 🟡 commencé (il reste des `⏳`) · ⬜ pas commencé

## Décision du Gate
<GO le <date> — offre vendue X fois, marketing prédictible, besoin de recruter>
ou <Pas encore le <date> — reprendre <étape amont>>

## Le goulot du moment  (module 3, à réviser chaque mois)
- <date> : <le goulot> → action en cours : <…>
- <date> : <le goulot précédent, levé>

## Priorités du trimestre en cours  (module 2)
1. <priorité> — responsable : <qui> — échéance : <date> — indicateur : <quoi>
2. …
3. …

## Journal des modules
- <date> — Module <n> validé. Ce qui a été tranché : <en une ligne>. Action verrouillée : <quoi, pour quand>.

## Points restés ouverts (`⏳`)
- <module> : <ce qui manque pour passer en ✅>
```

---

## Règles d'usage
- **Un module ne passe ✅** que si **toutes** les cases de sa checklist (`verification.md`) sont
  cochées. Sinon 🟡, et on nomme ce qui manque dans « Points restés ouverts ».
- Les colonnes **« Où il vit »** et **« Quand on le revoit »** ne sont pas décoratives : ce sont les
  briques 2 et 3 de la règle anti-PDF. **Une ligne sans ces deux colonnes remplies n'est pas
  implémentée.**
- Le **goulot se déplace** : garder l'historique plutôt que d'écraser, ça montre le chemin parcouru.
- À chaque reprise du parcours, `ctp-process` lit ce fichier **en premier** pour dire au membre où
  il en est et ce qui vient ensuite.
