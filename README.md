
# Détection de dérive par K-Means — Tableau de bord KPI

**Contexte** : Rapport de stage — OCP Jorf Lasfar, Unité UP-AP  
**Période** : Janvier 2024 – Décembre 2025  
**Outil** : Python 3 / Google Colab

## Objectif
Surveiller 8 KPIs industriels par clustering non supervisé (K-Means, K=3) afin de détecter automatiquement les zones : normal, dérive modérée et dérive critique. Comparaison avec le pilotage par seuil fixe ±10%.

## Contenu du notebook
- Import et nettoyage des données Excel
- Normalisation `StandardScaler` sur la baseline (Jan–Aoû 2024)
- Clustering K-Means individuel par KPI
- Tableau de bord visuel (heatmap + statut global mensuel)
- Métriques H2 (taux de détection, latence, couverture)
- Comparaison visuelle seuil fixe vs K-Means

## Fichiers principaux
- `K_Means_17.ipynb` : notebook complet (code + résultats + figures)
- Figures exportées : heatmap des zones, graphiques comparatifs H2

## Exécution
Ouvrir dans **Google Colab** ou **Jupyter Notebook**.  
Dépendances : `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `openpyxl`
