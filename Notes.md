# Gestion de projet  
## Introduction
Projet défini comme étant le résultat d'une **prise de décision**  produisant  un **résultat unique** dans une contraine temporelle et financière définie : 
```
Objectif - Délai - Budget
```
On le distinguera ainsi d'une tâche répétitive (i.e. support) ou d'une mission permanente.  
La méthode **agile** est présentée comme étant nettement plus efficace dans l'obtention de projet répondant aux satisfactions client. Toutefois elle nécessite un investissement temporel significatif côté client afin d'assurer la disponibilité nécessaire à l'agilité.  
<br>
Un projet sera considéré comme **non-conforme** si au moins l'une des trois contraintes n'est pas respectée.

## Organisation et méthodes
### Exemple d'un SI
Le rôle de la DSI sera d'apporter une réponse optimale aux besoin de traitement de l'information de l'entreprise.  

Son organisation comme sa taille dépendront de la nature et du coeur de métier de l'entreprise.
Définition des métiers **verticaux** (*e.g.* dev, assitance, helpdesk...) par opposition aux **tranversaux** (*e.g.* qualité, securité...)

### Organisation du projet
- **MOA** : Commanditaire du projet, ennonce les règles métier. Fixe les contraines. Peut être assitée par une *AMOA*.
- **MOE** : Equipe réaiisant le projet
- **Directeur vs. chef** de projet : selon la taille du projet. Assurera la coordination des différents chefs de projet.
- **Comité de projet** : Orientera les options proposées par les chefs de projet.
- **Comité de pilotage** : Assurera le suivi du projet par points d'étapes des chefs de projet.
- **ROI** : depense/economies-realisées/mois = N moins. Une bonne échelle de temps dans une entreprise établie sera de 3 ans.
- **ETP** : une personne à plein temps sur un projet.
<br>

La matrice **RACI** identifie les acteurs mobilisés sur et autour du projet :  
- Responsable de réalisation
- Approbateur : un seul approbateur par activité
- Consulté
- Informé  
<br>

|  Activité/Partenaire |  MOA | Equipe Projet  | DF  | Exploit-Inf  | SSI  |
|---|---|---|---|---|---|
| Collecter les besoins  | A  | R  |   |   |   |
| Analyser les besoins fonctionnels |  A | R  |  |   | C  |
| Analyser les besoins techniques  |  I |  R |  I | A  | C  |
| Acheter, installer et configurer un nouveau serveur    | I  |  A |  A/R | R  | R  |

Il faudra ici découper la dernière activité.  

<br>

**Etapes de gestion de projet**
```
1. Cadrage et choix de solution
2. Réalisation de tests
3. Recette et mise en production
```

**1. Cadrage et choix de solution**  
Realisation de **note de cadrage** (aka bon de commande, lettre de mission...) construite autour d'un avant projet.  
Chaque projet sera rattaché à un budget annuel de sa direction de référence.
<br>  
**2a. Réalisation : modèle en cascade**  
Importance de la création des spécifications techniques initiales.  
Plans de tests : d'**intégration** ou de **validation** (git, Jenkins et Selenium)  
Conception et développement  

**2b. Réalisation : modèle en V**  
On coupe le modèle cascade en plusieurs morceaux afin de rendre chaque élément réalisable en cascade.

**2b. Réalisation : modèle SCRUM**  
On découpe le projet en user Stories basées sur les actions utilisateurs qui seront liées à des techical stories.  
L'ensemble de stories s'appellant le product backlog.

**3. Recette et mise en production**  
Doc de recette  
<br>

### Cahier des charges et appel d'offre
Cahier des charges exprime le besoin, annexé au contrat

### Spécifications administratives
Sont gérées côté MAO.
<br>    

### TP : Systeme d'évaluation de cahier des charges AAP Gestion congés

1. Utilisation à distance
2. Utilsiation locale
3. ROI
4. Cout maintenance annuelle
5. Evolutivité
6. Accessibilité
7. Besoin de formation adoption
8. Nombre de clic pour valider la procédure
9. Cout stockage
10. Délai mise en prod

PBS : product breakdown structure. Déconstruire le projet pro en tache.

### TP utilisation de gantt project.

## Estimation de la charge
Attention la charge est en temps/homme, la durée en temps.  
Ronde Delphi
Methode d evaluation analytique : unité d'oeuvre à répartir en typologie de complexité qui associe à un degré (facile-normal-difficile) une certaine charge.

## Démarrage du projet

## Gestion des risques

| Risque  | Criticité  | Impact  | Probabilité  | Prévention  | Protection  | Détection  |
|---|---|---|---|---|---|---|
| Evolution règlementaire  | 8  | 4  | 2  | N/A  | Veille documentaire  | 3 => 24/125 |
| Reprise Covid  | 8  | 2  | 4  | Règles sanitaires, Vaccination  | Procédures télétravail  | 1 => 8/125 |
| Epidémie MonkeyPox  |  5 | 5  | 1  | Vaccination  | Veille info  | 4 => 20/125 |
| Augmentation Cout matériel | 16  | 4  | 4  | Budgetisation | Commande anticipées  | 2 => 32/125  |
|  Congé grossesse patho Marie|  9 | 3  | 3  | Paraige technique  | Remplacement  | 1 => 9/125  |

## Budget
Les RH sont un des pôles de dépense principaux. Pour chaque profil de salarié, le controlleur de gestion va écvaluer le cout moyen du profil.

Le calcul du coût total annuel : 
- CDA : 30k€ brut annuel + 50% de cs + 20% de couts de structure +30% ETP supports soit x2 salaire.  
- Calcul du coup d'un jour homme : Nb jours opérationnels/an. Soit ici 30k€*2/200 = 300j/an. Il faudra donc appliquer une marge à la tarification.

```
Cout total = Cout Jour Homme (Brut*charges/joursOp) * Nb j.h
```  
|Catégorie|	Nb J.h	|Salaire brut	|Facteur Charges|	Jours opérationnels	|Charges	|Charges tot	|Economie/mois
|---|---|---|---|---|---|---|---|							
|CDA	|130|	30000	|2|	200|	39000|	127000|	25000
|CP	|70	|40000|	2	|200	|28000|	**ROI**	|
|CPu	|50	|50000|	2	|200	|25000	|**5.08**|	
|Prestation|||||					20000	|	
Matériel|		|||			|15000	|	

## Bilan de projet
### Focus fait sur la réunion de débriefing.
Utilisation du KISS, Keep, Improve, Start, Stop sorte de SWOT agile.

## Qualité : Standart ISO-9000
On y distinguera un rôle **fournisseur** (*e.g.* équipe projet) et **client** (*e.g.* service rh). Les attentes et engagements des parties seront regroupés dans une convention/contrat de service (SLA : Service Level Agreement).  
**Plan d'assurance qualité** : description des actions apportant la qualité aux projets : réunion de lancement, de pilotage, documentation, audits de code source, N cas de test, revue de code source...  

Processus passera par PDCA (Plan Do Check Act) ou roue de Leming.

Le standart traite du management de la qualité et permet la certification au niveau de l'entreprise (certif ISO-9001). Il faut pour ce faire satisfaire 22 critères.

## Techniques de communication
