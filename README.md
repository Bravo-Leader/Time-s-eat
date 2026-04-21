# Time'Eats — Projet Collaboratif PMO

Référentiel documentaire complet pour le projet **Time'Eats** dans le cadre du cursus **CESI MAALSI — Semestre 2 (Avril 2026)**.

## Contexte

Time'Eats est un projet de système d'information de restauration d'entreprise. Ce dépôt contient l'ensemble des livrables de gestion de projet produits par la cellule PMO, couvrant les 5 phases du cycle de vie projet.

## Structure du dépôt

```
.
├── livrable_complet.tex        # Document maître compilant tous les livrables
├── livrable_complet.pdf        # PDF final du livrable complet
├── main.tex                    # Point d'entrée alternatif
├── cockpit_dsi.html            # Cockpit DSI (tableau de bord HTML)
├── diagramme_dependances.puml  # Diagramme de dépendances (PlantUML)
├── diagramme_gantt.puml        # Diagramme de Gantt (PlantUML)
├── diagramme_dependances.png   # Export PNG du diagramme de dépendances
├── diagramme_gantt.png         # Export PNG du diagramme de Gantt
├── contexte_timeEat.pdf        # Contexte du projet
├── style/                      # Styles LaTeX partagés (consulting.sty)
├── img/                        # Images et logos
└── referentiel/                # 22 templates PMO (voir ci-dessous)
```

## Référentiel documentaire — 22 templates PMO

| Fichier | Document | Phase |
|---------|----------|-------|
| P1-01 | Charte projet | Démarrage |
| P1-02 | Note de cadrage | Démarrage |
| P1-03 | Fiche d'identification | Démarrage |
| P1-04 | Matrice RACI | Démarrage |
| P2-05 | Plan de Management Projet (PMP) | Planification |
| P2-06 | WBS | Planification |
| P2-07 | Planning Gantt | Planification |
| P2-08 | Budget prévisionnel | Planification |
| P2-09 | Registre des risques | Planification |
| P2-10 | Plan de communication | Planification |
| P2-11 | Plan conduite du changement | Planification |
| P3-12 | Compte rendu de réunion | Exécution |
| P3-13 | Rapport d'avancement | Exécution |
| P3-14 | Demande de changement | Exécution |
| P3-15 | Log des anomalies | Exécution |
| P4-16 | Tableau de bord projet | Maîtrise |
| P4-17 | Rapport d'écarts | Maîtrise |
| P4-18 | Compte rendu COPIL | Maîtrise |
| P5-19 | PV de recette fonctionnelle | Clôture |
| P5-20 | PV de recette technique | Clôture |
| P5-21 | Rapport de clôture | Clôture |
| P5-22 | PV de transfert en exploitation | Clôture |
| P5-23 | Fiche REX | Clôture |

Les PDFs compilés sont disponibles dans `referentiel/pdf/`.

## Compilation LaTeX

Chaque template se compile indépendamment :

```bash
cd referentiel
pdflatex P1-01_charte_projet.tex
```

Pour le livrable complet :

```bash
pdflatex livrable_complet.tex
biber livrable_complet
pdflatex livrable_complet.tex
```

## Technologies

- **LaTeX** — rédaction et mise en page des livrables
- **PlantUML** — diagrammes de dépendances et Gantt
- **HTML/CSS** — cockpit DSI interactif

## Auteurs

Cellule PMO — CESI MAALSI 2026
