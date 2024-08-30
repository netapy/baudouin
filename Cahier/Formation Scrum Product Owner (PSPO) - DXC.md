---
Created: 2021-10-12T09:30
tags:
  - Cours
  - Work
---
> [!important]  
> Formation sur 3 jours répartis jusqu'au 10 novembre.  
---
## Supports du cours :
![[Guide_Scrum_2020_fr.pdf]]
![[Support_Mthodes_agiles_-_Scrum.docx]]
---


# Qu'est-ce que l'AGILE ?
L'AGILE est un concept et non pas une méthode ⇒ les méthodes d'application de l'AGILE sont diverses. En l'occurence on apprend la méthode **SCRUM**.
### Pour la certification :
On part du principe qu'on est dans un monde 100% Agile **OR** dans la réalité on est jamais sur un Agile parfait mais plutôt un mélange hybride avec du Cycle en V ou autres.
### Le cycle en V :
Les phases sont **séquentielles** et chaque phase du projet est **prévisible**. Tout est décrit en amont dans un plan de management du projet.
==**Inconvénient**== ⇒ Il n'y a pas de permanence, rien n'est définitif et il faut prévoir le changement.
L'agile permet de compenser 3 grands défauts (80% des échecs dues à ces facteurs) :
- **L'effet tunnel :** l'équipe ne s'adapte pas aux changements d'environnement, conforme aux attentes mais décalé par rapport à la réalité (cause majeure d'échecs).
- **Documentation** : le non dit, prévaut sur le dit. La documentation est en concurrence avec la qualité du produit. C'est 80% du travail sur certains projets.  
    En agile on créer la documentation en fonction de ce qui est affiché, et non l'inverse.  
    IKIWISI → I'll know it when i see it.  
    
- **Management de risque** : La probabilité est une constante / l'impact est croissant en fonction de l'avancée du projet
Le **_Chaos Report_** répertorie les projets industriels qui ont échoué et analyse la cause des échecs. La méthodologie **_PrincE2_** a pour vocation de pallier à 80% de ces problèmes.
On dit qu'un projet est réussi lorsqu'il rapport au moins la moitié du retour sur investissement initialement prévu.
### Manifeste pour le développement Agile de logiciels valorise 4 valeurs :
- Les individus et leurs interactions (plus que le process & outils)
- Des logiciels opérationnels (plus qu'une documentation exhaustive)
- La collaboration avec les clients (plus que la négociation contractuelle) (**⇒ le rôle du** **product owner** **a été créé pour respecter cette valeur du manifeste)**
- L'adaptation au changement (plus que le suivi d'un plan)

> [!important]  
> Le manifeste est la base de l'agilité, il faut l'avoir lu plusieurs fois pour passer la certification, notamment les 12 principes du manifeste.  
L'agile met un point d'accent sur la **durée de travail** qui doit être régulière (non pas pour des raisons de bien-être, mais pour des raisons de référence de temps). Il faut garder une référence précise pour la quantité quotidienne de travail réalisable.
  
Le cycle de développement Agile est :
- **Itératif** (composé d'itérations) : chaque itération est un mini projet en soi. Durée courte de qq semaines et définie à l'avance.
- **Incrémental** (chaque itération ajoute une fonctionnalité exploitable)
- **Adaptatif** (prend en compte les exigences du client à tout moment)
### L'historique des types de management :
- 1960 → Contrôleur _(taylorisme)_
- 1980 → Leader _(taylorisme)_
- 2000 → Facilitateur _(agilité)_
- 2010 → Co-opté _(entreprise libérée)_
Un manager agile co-opt les membres de son équipe.
![[/Untitled 7.png|Untitled 7.png]]
---
# Scrum : le process
1. **Sprint 0 :** défini la nature du sprint
    - Artefact : Product Backlog
2. **Sprint Planning Meeting 1/2** : définition des chantiers du backlog à suivre lors du sprint.
    - Artefact : Sprint Backlog
3. **Sprint Planning Meeting 2/2** : décomposition des chantiers séléctionnés en tâches
    - Artefact : Sprint Backlog
4. **Sprint :** Daily scrum chaque matin / environ 3 semaines
    - Artefact : BurnDown Chart
5. **Sprint Review / Demo** : description du produit après incrémentation. Permet de synchroniser les équipes (développeurs) sur la version en cours.
    - Artefact : BurnUp Chart
6. **Sprint Retrospective**

> [!important]  
> En scrum on ne parle pas de livrable mais d'artefact.  
## Terminologie :
- **Development Team** —> les developeurs
- **La Team** —> développeurs + scrum master (nb: personne ne peut diriger la team, elle est indépendant et en auto-gestion)
- **Scrum Team** —> développeurs + scrum master + product owner
- **Release** —> version du projet
  
---
## Exercice 1 — équipe n°2
![[/Untitled 1 2.png|Untitled 1 2.png]]
Format de l'outil —> **logiciel interne**
### 5 fonctionnalités principales :
1. Saisie des évènements/lieu dans une base de données
    - En tant que **organisateur** je veux **retrouver les évènements & lieux** afin d'**organiser et suivre les évènements passés et à venir.**
1. Saisie du matériel/logistique (tréteaux, bancs etc...)
    - En tant que **organisateur** je veux **lister le matériel à disposition** afin d'**assurer leur répartition sur les évènements.**
1. Outil de comptabilité des recettes de l'activité
    - En tant que **organisateur** je veux **pouvoir suivre la comptabilité des évènements** afin de **déterminer la rentabilité de l'activité.**
2. Outil de gestion des contacts (hôtes, propriétaires de jardin...)
    - En tant que **organisateur** je veux **centraliser ma base de contacts** afin de **faciliter la mise en relation avec les interlocuteurs**.
1. Base des textes/pièces/représentations de la troupe
    - En tant qu'**acteur** je veux **centraliser les différents textes des représentations** afin de **pouvoir les consulter de façon dématérialisée.**
  
_Bonus :_
1. Outil de centralisation des retours du public & hôtes (capitalisation des expériences)
2. Service de messagerie entre les acteurs
  
---
  
En agile, c'est les **experts** (équipes de développement) qui **constitue** **l'offre** — il propose au client les fonctionnalités à développer → Marketing de l'offre.
4 phases dans un projet :
- exposition
- production
- restitution
- catégorisation
Le **product backlog** est un tableau contenant l'ensemble des idées de fonctionnalités du produit générées par l'équipe.
  
Pour exprimer des exigences :
- **Description statique** (vue de l'extérieur) — on décrit la technologie et les moyens utilisés pour réaliser le produit (moteur, roues, structure...).
- **Description dynamique** (vue de l'intérieur) — on décrit l'usage qui est fait par l'utilisateur.
Il existe plusieurs modèles, **il appartient à l'équipe de décider la méthode de hiérarchisation** à utiliser pour les exigences.
![[/Untitled 2 3.png|Untitled 2 3.png]]
**Quels sont les 33 piliers de Scrum ?**
—>Transparence, l’inspection, l’adaptation
Au cours d’un sprint on ne modifie pas l’organisation établie.
Artefact : product backlog, sprint backlog et charts