# Analyse-e-commerce
Analyse de ventes pour un e-commerce
Voici une proposition de structure complète pour le fichier **README.md** de ton projet. Ce document est conçu pour être à la fois professionnel, clair et structuré, idéal pour documenter ton travail (par exemple pour un projet OpenClassrooms/FAO).

---

# 📝 README.md

# Étude de la Sous-Nutrition dans le Monde (Données Historiques 2013-2017) — Organisation des Nations Unies (FAO)

## 📌 Présentation du Projet

Ce projet s'inscrit dans le cadre des missions de l'**Organisation des Nations Unies pour l'alimentation et l'agriculture (FAO)**, dont l'objectif fondamental est d'aider à construire un monde libéré de la faim.

Suite à la mutation de notre ancien Data Analyst Julien, l'équipe menée par Marc (chercheur en économie de la santé) reprend une étude de grande ampleur sur la sous-nutrition mondiale. Alors que la période récente (2018 à nos jours) a déjà été couverte, ce volet du projet se concentre sur l'**analyse historique des données de 2013 à 2017**.

---

## 🎯 Objectifs de la Mission

L'objectif principal est de réaliser une analyse statistique approfondie pour dresser un état des lieux de la malnutrition globale sur la période historique ciblée.

### 📊 Analyses principales à réaliser :

* **Proportion de la population mondiale** en état de sous-nutrition.
* **Nombre total d'êtres humains** en situation de sous-nutrition.
* **Identification des pays** les plus touchés par la famine (en taux et en volume).
* **Analyse de la disponibilité alimentaire** par habitant et comparaison avec les besoins réels.
* **Évaluation des pertes alimentaires** et de l'utilisation des céréales (alimentation humaine vs. animale).

---

## 📁 Structure des Données

Le projet s'appuie sur quatre fichiers de données principaux fournis en pièces jointes :

* `aide_alimentaire.csv` : Suivi des aides humanitaires par pays et par année.
* `dispo_alimentaire.csv` : Détail des disponibilités alimentaires par produit et par pays (en calories, protéines, etc.).
* `insuffisance_nutritionnelle.csv` : Nombre de personnes en état de sous-nutrition (moyennes glissantes).
* `population.csv` : Données démographiques mondiales par pays et par année.
* `lexique.pdf` : Dictionnaire des termes techniques (Disponibilité intérieure, Semences, Pertes, etc.).

---

## 🛠️ Stack Technique & Installation

> **Note sur le choix technologique :** Bien que Julien ait laissé le choix ouvert entre R et Python, ce projet sera réalisé en **Python** pour sa robustesse en manipulation de données (Pandas) et sa flexibilité en visualisation.

### Prérequis

Pour exécuter le notebook d'analyse, vous devez installer les bibliothèques suivantes :

```bash
pip install pandas numpy matplotlib seaborn

```

### Lancement

1. Clonez ce dépôt.
2. Placez les fichiers `.csv` dans un dossier nommé `data/`.
3. Ouvrez le notebook principal :

```bash
jupyter notebook analyse_historique_FAO.ipynb

```

---

## 📈 Plan d'Analyse (Notebook)

Le notebook préparé par Julien suit les étapes standardisées du cycle de vie de la Data :

1. **Nettoyage des données :** Gestion des valeurs manquantes, conversion des types (notamment les chaînes de caractères `<0.1` ou `N/A`), et harmonisation des unités.
2. **Jointures :** Centralisation des tables (Population, Disponibilité, Insuffisance) pour permettre les calculs croisés.
3. **Exploration & Analyses :** Réponse aux questions clés de Marc.
4. **Analyses complémentaires (Bonus) :** Focus sur la corrélation entre le PIB des pays et leur taux de sous-nutrition.

---

## 👥 Membres de l'Équipe

* **Marc** : Responsable d'équipe / Chercheur en économie de la santé.
* **Julien** : Data Analyst (Auteur de la partie 2018+ & de l'ébauche de présentation).
* **Vous** : Data Analyst en charge de la période historique 2013-2017.

---

### 💬 Ma réponse à Marc concernant le choix du langage :

> *"Merci pour ton accueil, Marc ! Je suis ravi de rejoindre l'équipe sur un sujet aussi crucial. Pour répondre à ta question : **j'ai une préférence pour Python**. Sa bibliothèque Pandas est parfaite pour manipuler efficacement les jointures complexes de ce dataset, et cela me permettra de nettoyer proprement les types de données que Julien a soulignés dans ses commentaires. Je me lance de ce pas dans l'analyse de son ébauche et du notebook !"*
