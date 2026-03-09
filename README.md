# 🏢 Prédiction de Consommation Énergétique des Bâtiments

Analyse et modélisation supervisée de la consommation énergétique des bâtiments non-résidentiels basée sur les données de benchmarking énergétique de 2016.

## 📋 Contexte

Ce projet vise à développer un modèle prédictif pour estimer la consommation énergétique (Site Energy Use) des bâtiments non-résidentiels. Les données proviennent d'un dataset public de benchmarking énergétique contenant des informations détaillées sur la consommation énergétique, les caractéristiques des bâtiments et leurs émissions de gaz à effet de serre.

## 📊 Données

**Fichier principal :** `2016_Building_Energy_Benchmarking.csv`

### Caractéristiques principales :
- **Période :** 2016
- **Scope :** Bâtiments non-résidentiels
- **Variables clés :**
  - `PropertyGFATotal` : Surface totale du bâtiment (en pieds carrés)
  - `SiteEnergyUse(kBtu)` : Consommation énergétique totale (cible à prédire)
  - `SiteEUI(kBtu/sf)` : Intensité énergétique par unité de surface
  - `Electricity(kWh)` : Consommation électrique
  - `NaturalGas(therms)` : Consommation de gaz naturel
  - `YearBuilt` : Année de construction
  - `ENERGYSTARScore` : Score ENERGY STAR du bâtiment
  - `TotalGHGEmissions` : Émissions totales de gaz à effet de serre

### Traitement des données :
- ✅ Filtrage des bâtiments non-résidentiels uniquement
- ✅ Suppression des colonnes constantes ou inutiles
- ✅ Gestion des données manquantes
- ✅ Analyse exploratoire (visualisations, statistiques descriptives)

## 🎯 Objectifs

1. **Exploration et nettoyage des données** : Comprendre la structure, identifier les anomalies et préparer les données
2. **Analyse exploratoire (EDA)** : Visualiser les distributions, les relations entre variables et détecter les phénomènes clés
3. **Modélisation supervisée** : Développer un modèle de régression pour prédire la consommation énergétique
4. **Évaluation et optimisation** : Évaluer les performances du modèle et l'optimiser au besoin

## 📁 Structure du Projet

```
building_conso_data_predict/
├── README.md                                          # Ce fichier
├── 2016_Building_Energy_Benchmarking.csv             # Données brutes
└── P3_template_modelistation_supervisee_data_scientist.ipynb  # Notebook principal
```

## 🚀 Comment utiliser

### Prérequis
- Python 3.7+
- Jupyter Notebook/Lab
- Librairies Python :
  - `pandas` : Manipulation et analyse de données
  - `matplotlib` : Visualisations
  - `seaborn` : Visualisations avancées
  - `scikit-learn` : Modélisation supervisée

### Lancer le projet

1. Ouvrir le notebook Jupyter :
   ```bash
   jupyter notebook P3_template_modelistation_supervisee_data_scientist.ipynb
   ```

2. Suivre les sections du notebook dans l'ordre :
   - **Analyse Exploratoire** : Charger et explorer les données
   - **Préparation des Données** : Nettoyer et transformer
   - **Modélisation Supervisée** : Entraîner et évaluer le modèle

## 📈 Étapes principales du Notebook

### 1. Import des modules
Chargement des librairies nécessaires pour l'analyse et la modélisation.

### 2. Analyse Exploratoire (EDA)
- Aperçu des données (`head()`, `info()`)
- Analyse des valeurs manquantes
- Identification des colonnes constantes/quasi-constantes
- Visualisations des distributions clés
  - Distribution de l'année de construction
  - Relation entre surface et consommation énergétique

### 3. Filtrage et préparation
- Filtrage des bâtiments non-résidentiels
- Suppression des colonnes inutiles
- Préparation pour la modélisation

### 4. Modélisation Supervisée
*À compléter lors de la continuation du projet*

## 📊 Visualisations principales

- **Histogramme** : Distribution de l'année de construction
- **Scatter plot** : Relation logarithmique entre surface (PropertyGFATotal) et consommation (SiteEnergyUse)

## 🔍 Points clés découverts

1. Les bâtiments plus anciens (construits avant 1980) représentent une part significative du dataset
2. Une relation quasi-logarithmique existe entre la surface du bâtiment et sa consommation énergétique
3. Plusieurs colonnes constantes (DataYear, State) ont été supprimées car elles n'apportent pas d'information
4. Les données manquantes sont inégalement distribuées selon les colonnes

## 📝 Notes pour la continuation

- [ ] Compléter l'analyse exploratoire avec d'autres visualisations
- [ ] Analyser les corrélations entre features et la cible
- [ ] Gérer les valeurs manquantes (suppression, imputation, etc.)
- [ ] Sélectionner les features pertinentes
- [ ] Entraîner plusieurs modèles de régression
- [ ] Évaluer les modèles (RMSE, R², MAE, etc.)
- [ ] Optimiser les hyperparamètres
- [ ] Analyser l'importance des features

## 📖 Ressources utiles

- [ENERGY STAR Portfolio Manager](https://portfoliomanager.energystar.gov/)
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)

## ✨ Auteur

Projet d'apprentissage - OpenClassroom Data Science

---

**Dernière mise à jour :** Mars 2026
