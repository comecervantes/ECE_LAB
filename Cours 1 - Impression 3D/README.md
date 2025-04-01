#  Formation Modélisation 3D & Impression 3D FDM

## Sommaire

1. [Introduction](#introduction)  
2. [Outils de mesure et de conception](#2--outils-de-mesure-et-de-conception)  
   2.1 [Les instruments de mesure](#21--les-instruments-de-mesure)  
   2.2 [Types de logiciels](#22--types-de-logiciels)  
   2.3 [Outils utilisés dans cette formation](#23--outils-utilisés-dans-cette-formation)  
3. [Modélisation 3D](#3--modélisation-3d)  
   3.1 [Prise en main d’Onshape](#31--prise-en-main-donshape)  
   3.2 [Projet d’exemple : Reproduction d’un décapsuleur](#32--projet-dexemple--reproduction-dun-décapsuleur)  
4. [Impression 3D : les bases](#4--impression-3d--les-bases)  
   4.1 [Types d’imprimantes](#41--types-dimprimantes)  
   4.2 [Comparatif des technologies](#42--comparatif-des-technologies)  
   4.3 [Additif vs Soustractif](#43--additif-vs-soustractif)  
5. [Matériaux pour FDM](#5--matériaux-pour-fdm)  
   5.1 [Tableau comparatif](#51--tableau-comparatif)  
   5.2 [Conseils de choix](#52--conseils-de-choix)  
   5.3 [Stockage des filaments](#53--stockage-des-filaments)  
6. [Les slicers (trancheurs)](#6--les-slicers-trancheurs)  
   6.1 [Rôle d’un slicer](#61--rôle-dun-slicer)  
   6.2 [Réglages essentiels à connaître](#62--réglages-essentiels-à-connaître)  
   6.3 [Motifs de remplissage](#63--motifs-de-remplissage)  
7. [Projet d’optimisation d’impression](#7--projet-doptimisation-dimpression)  
8. [Contact et remerciements](#8--contact-et-remerciements)

## Introduction

Bienvenue dans ce module d’introduction à la **modélisation 3D** et à **l’impression 3D FDM**.  
Ce document accompagne une présentation conçue pour vous donner les **bases solides** de la modélisation numérique, de la compréhension des machines de fabrication additive, et du processus complet allant de la conception à l’objet physique imprimé.

Ce cours vous permettra de :

- Comprendre les différences entre les types de modélisation (technique vs artistique)
- Découvrir les principaux logiciels utilisés (CAO, DAO)
- Prendre en main un outil en ligne gratuit : **Onshape**
- Savoir préparer un modèle pour l’impression via un **slicer**
- Comprendre les **réglages clés** d’une impression FDM
- Choisir le **bon matériau** selon l’usage
- Réaliser un projet concret d’**optimisation d’impression**

L’approche est volontairement **progressive et accessible**, avec des exemples concrets et reproductibles.

--- 

##  Ce dont vous avez besoin

- Un **ordinateur** avec connexion Internet
- Un **compte étudiant Onshape** (gratuit)
- Le logiciel **Bambu Studio** installé (ou un autre slicer)
- Une **imprimante FDM** (ou accès à une imprimante via un fablab ou celle de l'école)

---

## 📎 Ressources du cours

📦 Dépôt GitHub : [ECE_LAB](https://github.com/comecervantes/ECE_LAB.git)  
🌐 Onshape : [https://www.onshape.com](https://www.onshape.com)  
🧵 Bambu Studio : [https://bambulab.com/fr-fr/download/studio](https://bambulab.com/fr-fr/download/studio)  
📚 Modèles 3D libres : [MakerWorld](https://makerworld.com/fr), [Thingiverse](https://www.thingiverse.com)

---

## 2.  Outils de mesure et de conception

### 2.1  Les instruments de mesure

En modélisation comme en fabrication, il est crucial de **mesurer avec précision**. L’outil principal est :

#### ▸ Pied à coulisse

Le pied à coulisse permet trois types de mesures :

- **Mesure extérieure** : diamètre ou largeur d’une pièce (ex : tige, tube…)
- **Mesure intérieure** : diamètre d’un trou ou espace entre parois
- **Mesure de profondeur** : fond d’un trou, hauteur d’un logement

C’est un instrument indispensable pour **reproduire des objets physiques** en 3D avec justesse.

---

### 2.2  Types de logiciels

Il existe deux grandes familles de logiciels pour modéliser en 3D :

#### ▸ CAO — *Conception Assistée par Ordinateur*

Utilisée pour des besoins **techniques et fonctionnels**, la CAO permet :

- La conception de **pièces mécaniques**
- L’**assemblage** de composants
- Des **tests de contraintes**, mouvements, collisions
- Des exportations en format **.STL** pour l’impression

**Exemples** : SolidWorks, Fusion 360, FreeCAD, Onshape

#### ▸ DAO — *Dessin Assisté par Ordinateur*

La DAO est orientée vers la **création artistique ou visuelle**, utilisée pour :

- Créer des objets aux formes libres (sculpture 3D, animation)
- Produire des **rendus réalistes**
- Concevoir des scènes, textures, lumières…

**Exemple principal** : Blender

---

### 2.3  Outils utilisés dans cette formation

Pour cette session, nous utilisons principalement :

#### ✅ Onshape
- Logiciel **en ligne**, gratuit pour les étudiants
- Permet de modéliser rapidement et d'apprendre les bases de la CAO
- Nécessite juste un compte étudiant pour commencer

#### ✅ Bambu Studio
- Logiciel de **slicing** pour préparer les impressions FDM
- Compatible avec d’autres imprimantes via export G-code
- Permet de paramétrer l’impression, le remplissage, les supports, etc.

---

## 3.  Modélisation 3D

### 3.1  Prise en main d’Onshape

#### ▸ Interface
Onshape propose une interface similaire à celle des logiciels professionnels comme SolidWorks, avec :
- Une **barre d’outils d’esquisse** (traits, cercles, cotes…)
- Une **barre d’outils de modélisation** (extrusion, révolution, chanfrein…)
- Un **arbre de construction** pour visualiser les étapes

#### ▸ Fonctionnalités de base
Les opérations principales à maîtriser :
- **Créer une esquisse** sur une face ou un plan
- **Contraindre** une esquisse (dimensions, relations)
- **Extruder** ou **réaliser une révolution** pour créer du volume
- Utiliser **des opérations booléennes** (ajout, retrait, intersection)

---

### 3.2  Projet d’exemple : Reproduction d’un décapsuleur

####  Objectif
Reproduire un **modèle simple** issu d'une banque de fichiers 3D (MakerWorld) afin d'apprendre à utiliser les outils de base de la modélisation.

🔗 Modèle original :  
[Décapsuleur porte-clés - MakerWorld](https://makerworld.com/fr/models/138919-bottle-beer-opener-keychain?from=search)

####  Étapes typiques :
1. Importer l’image ou les mesures du modèle à reproduire
2. Réaliser une esquisse de profil sur un plan
3. Extruder le volume principal
4. Ajouter les détails (trous, chanfreins…)
5. Exporter en .STL pour impression

#### ✅ Objectifs pédagogiques :
- Comprendre la logique **esquisse → volume**
- Savoir utiliser les **contraintes géométriques**
- Gérer les **unités, tolérances et symétries**
- Apprendre à **préparer un fichier pour l’impression**

Ce mini-projet est idéal pour se familiariser avec le logiciel tout en créant un objet fonctionnel.

---

## 4.  Impression 3D : les bases

L’impression 3D, ou fabrication additive, est un processus de création d’objets physiques par ajout successif de couches de matière. Il existe plusieurs technologies, mais ici nous nous concentrerons principalement sur le procédé **FDM**.

### 4.1  Types d’imprimantes

#### ▸ FDM – Fused Deposition Modeling
- Fonctionnement : extrusion de filament plastique chauffé, couche par couche
- Matériaux : PLA, ABS, PETG, TPU, etc.
- Avantages : accessible, économique, polyvalent
- Inconvénients : qualité moyenne, visiblement strié

#### ▸ SLA – Stéréolithographie
- Fonctionnement : durcissement de résine liquide par un laser UV
- Avantages : précision très fine, surface lisse
- Inconvénients : post-traitement, résine coûteuse, toxique

#### ▸ SLS – Selective Laser Sintering
- Fonctionnement : frittage de poudre plastique par laser
- Avantages : pas besoin de supports, haute résistance, détails fins
- Inconvénients : coûteux, usage industriel, machine encombrante

---

### 4.2  Comparatif des technologies

| Technologie | Matériau         | Précision     | Coût      | Complexité | Idéal pour                           |
|-------------|------------------|---------------|-----------|------------|--------------------------------------|
| **FDM**     | Filament (PLA…)  | Moyenne       | €         | Faible     | Prototypes, objets fonctionnels      |
| **SLA**     | Résine liquide    | Très élevée   | €€€       | Moyenne    | Miniatures, objets décoratifs        |
| **SLS**     | Poudre de nylon   | Élevée        | €€€€      | Haute      | Pièces techniques, petites séries    |

---

### 4.3  Additif vs Soustractif

| Fabrication additive          | Fabrication soustractive         |
|-------------------------------|----------------------------------|
| Ajout de matière (couche par couche) | Retrait de matière (usinage, découpe) |
| Moins de gaspillage          | Haute précision                  |
| Formes complexes possibles   | Finitions très nettes            |
| Ex : FDM, SLA, SLS           | Ex : Fraiseuse CNC, découpe laser |

---

L'impression 3D FDM est idéale pour **prototyper rapidement**, tester des idées, et produire des objets à moindre coût, tout en apprenant les bases de la fabrication numérique.

---

## 5.  Matériaux pour FDM

Le choix du matériau est un paramètre clé en impression 3D FDM. Chaque filament possède des propriétés mécaniques, thermiques et esthétiques spécifiques. Voici un aperçu des principaux matériaux utilisés.

### 5.1  Tableau comparatif

| Matériau      | Facilité d'impression | Solidité | Souplesse | Résistance thermique | Particularités | Applications typiques |
|---------------|------------------------|----------|-----------|-----------------------|----------------|------------------------|
| **PLA**       | ⭐⭐⭐⭐                  | ⭐⭐       | ❌         | ⭐⭐                    | Biodégradable, rigide, couleurs variées | Prototypes visuels, déco, figurines |
| **ABS**       | ⭐⭐                    | ⭐⭐⭐⭐     | ⭐         | ⭐⭐⭐⭐                 | Résistant aux chocs et à la chaleur, dégage des fumées | Pièces techniques, boîtiers |
| **PETG**      | ⭐⭐⭐⭐                  | ⭐⭐⭐⭐     | ⭐⭐        | ⭐⭐⭐                  | Résistant à l'humidité, bon compromis solidité/facilité | Pièces fonctionnelles, contenants |
| **TPU/TPE**   | ⭐⭐                    | ⭐⭐       | ⭐⭐⭐⭐      | ⭐⭐                    | Très souple, effet caoutchouc | Joints, semelles, protections |
| **Nylon**     | ⭐                     | ⭐⭐⭐⭐⭐   | ⭐⭐⭐       | ⭐⭐⭐⭐                 | Très solide, sensible à l'humidité | Engrenages, pièces mécaniques |
| **Composites**| ⭐⭐⭐                   | ⭐⭐⭐⭐     | ❌         | ⭐⭐⭐                  | Mélange PLA + fibres (carbone, bois, métal…) | Objets design, rigides |

---

### 5.2  Conseils de choix

-  **Débutant ?** → Choisis le **PLA** : facile à imprimer, pas de plateau chauffant requis.
-  **Besoin de solidité ?** → Oriente-toi vers le **PETG** ou le **Nylon** (si tu maîtrises bien la machine).
-  **Souplesse requise ?** → Le **TPU** est parfait, mais demande une imprimante bien réglée.
-  **Esthétique originale ?** → Les **PLA composites** offrent des rendus uniques (effet bois, bronze…).

---

### 5.3  Stockage des filaments

Certains filaments (notamment **Nylon** et **TPU**) sont très sensibles à l’humidité. Il est conseillé de :

- Les stocker dans des **boîtes hermétiques avec du gel de silice**
- Les sécher avant usage si nécessaire (déshumidificateur ou four à basse température)

---

Connaître les propriétés des matériaux permet d’adapter ses impressions aux besoins réels : solidité, souplesse, coût, esthétique ou facilité d'impression.

---

## 6.  Les slicers (trancheurs)

Le slicer est le logiciel qui prépare un modèle 3D pour l'impression. Il convertit le fichier `.STL` ou `.3MF` en **G-code**, le langage lu par l'imprimante 3D.

### 6.1  Rôle d’un slicer

- Tranche l’objet 3D en **couches horizontales**
- Génère le **chemin d’impression** pour la buse
- Paramètre la température, la vitesse, le remplissage, les supports, etc.
- Optimise les temps, le coût, et la qualité d’impression

**Exemples de slicers :**  
- Bambu Studio (utilisé ici)  
- Cura (Ultimaker)  
- PrusaSlicer  
- OrcaSlicer

---

### 6.2  Réglages essentiels à connaître

Voici les 10 réglages clés à maîtriser dans un slicer :

1. **Épaisseur de couche (Layer height)**  
   → Détermine la résolution verticale de l’impression (ex : 0.2 mm standard)

2. **Taux de remplissage (Infill)**  
   → % de matière à l’intérieur (ex : 15%, 30%, 100%)

3. **Parois / Coques (Wall thickness)**  
   → Nombre de contours solides de la pièce (ex : 2–3 murs)

4. **Température de la buse (Nozzle temperature)**  
   → Dépend du filament (ex : PLA ≈ 200°C)

5. **Température du plateau (Bed temperature)**  
   → Aide à l’adhérence (ex : PLA ≈ 60°C)

6. **Adhérence au plateau (Bed adhesion)**  
   → Brim, raft ou skirt pour éviter le décollement

7. **Vitesse d’impression (Print speed)**  
   → Plus rapide = gain de temps mais perte de qualité

8. **Supports (Supports)**  
   → Structures temporaires pour maintenir les parties en surplomb

9. **Rétraction (Retraction)**  
   → Tire légèrement le filament pour éviter les fils entre deux zones

10. **Orientation de la pièce (Part orientation)**  
    → Optimise les supports, la solidité et la qualité visuelle

---

### 6.3  Motifs de remplissage

Certains motifs influencent la solidité, le poids et le temps d’impression :

| Motif          | Description                            | Solidité |
|----------------|----------------------------------------|----------|
| **Grid**       | Grille simple, rapide                  | ⚠️ Moyenne |
| **Honeycomb**  | Nid d’abeille, léger et résistant      | ✅ Bonne |
| **Gyroid**     | Forme organique, très robuste          | 💪 Excellente |
| **Cubic**      | Remplissage 3D structuré               | ✅ Bonne |

💡 Le choix du **motif** et du **taux de remplissage** impacte directement la résistance de la pièce et son temps d’impression.

---

Maîtriser un slicer permet d’exploiter au maximum les capacités de votre imprimante FDM et d’ajuster les impressions selon vos objectifs : rapidité, solidité, esthétique ou économie de matériau.

---

## 7.  Projet d’optimisation d’impression

###  Objectif

L’objectif de ce mini-projet est de comprendre comment optimiser une impression 3D en jouant sur les paramètres du slicer.  
On cherche à **réduire le poids, le coût et le temps d’impression**, sans altérer la fonction principale de l’objet.

---

###  Cas d’étude : un décapsuleur imprimé avant et après optimisation

| Critère                | Avant optimisation | Après optimisation | Amélioration (%) |
|------------------------|--------------------|---------------------|------------------|
| **Poids**              | 10,63 g            | 5,10 g              | –52,0 %          |
| **Coût matière**       | 0,21 €             | 0,10 €              | –52,4 %          |
| **Temps d’impression** | 34 min 50 s        | 26 min 58 s         | –22,6 %          |

---

###  Méthode d’optimisation

Les ajustements effectués dans le slicer ont porté sur :

- **Réduction du taux de remplissage** (passage de 30 % à 15 %)
- **Changement du motif de remplissage** (ex : Grid → Gyroid)
- **Réduction du nombre de parois** (3 → 2)
- **Ajustement de l’orientation de la pièce** pour minimiser les supports
- **Suppression des supports inutiles**

---

### ✅ Résultat

Grâce à ces réglages, on obtient un gain significatif sur tous les aspects :

- Moins de matière utilisée = économie de filament
- Temps d’impression réduit = gain de productivité
- Résultat visuel et fonctionnel **identique au modèle original**

Ce projet montre l’importance de bien comprendre et ajuster les paramètres d’un slicer pour rendre l’impression plus **efficace, économique et durable**.

---

## 8.  Contact et remerciements

Ce document a été réalisé dans le cadre d’une **séance de tutorat** à destination des étudiants de l’ECE, afin de leur faire découvrir la **modélisation 3D** et l’**impression FDM** à travers un projet concret.

###  Contact

Réalisé par **Côme Cervantes**  
📧 [come.cervantes@edu.ece.fr](mailto:come.cervantes@edu.ece.fr)  
🌐 [GitHub - comecervantes](https://github.com/comecervantes)  
🔗 [LinkedIn - Côme Cervantes](https://www.linkedin.com/in/côme-cervantes/) 

N’hésitez pas à me contacter pour toute question, suggestion ou collaboration autour des sujets de prototypage, modélisation ou impression 3D.

---

Merci pour votre attention et bonne création !
