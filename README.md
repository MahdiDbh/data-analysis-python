# data-analysis-python — Analyse de Données en Python

Travaux pratiques et projet d'analyse de données réalisés avec Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy).

**Auteur :** DEBBAH Islam Mahdi

---

## Structure du projet

```
ADPython/
├── TP1.ipynb                  # Travaux pratiques — Exercices 1 & 2
├── projet_spotify.ipynb       # Projet — Analyse de tendances Spotify
├── CarPrice_Assignment.csv    # Dataset : prix de voitures (164 entrées, 26 colonnes)
├── employment.csv             # Dataset : taux d'emploi par secteur (2000–2010)
├── unemployment.csv           # Dataset : chômage
├── penguins.csv               # Dataset : pingouins
├── consommation_energie.csv   # Dataset : consommation énergétique
└── spotify.csv                # Dataset : 2000 morceaux Spotify
```

---

## TP1 — Exercices d'analyse exploratoire (EDA)

### Exercice 1 : Dataset CarPrice (`CarPrice_Assignment.csv`)

- Chargement et exploration générale (164 lignes × 26 colonnes)
- Statistiques descriptives sur la variable `price`
- Sélection des colonnes numériques (16 variables)
- Matrice de corrélation avec heatmap
- Histogramme et boxplot de la distribution des prix

### Exercice 2 : Dataset Employment (`employment.csv`)

- Chargement et inspection des données (122 lignes × 17 colonnes)
- Vérification et traitement des valeurs manquantes et doublons
- Détection des outliers par méthode IQR sur tous les secteurs
- Visualisation de l'évolution des secteurs Construction, Finance, Education & Health
- Analyse statistique complète du secteur Finance (moyenne, médiane, skewness, kurtosis)
- Corrélation de Finance avec toutes les autres variables
- Filtrage des données pour l'année 2005

---

## Projet — Analyse de tendances Spotify (`projet_spotify.ipynb`)

Analyse complète d'un dataset de 2000 morceaux Spotify (après suppression de 59 doublons).

### Partie 1 : Analyse des données

| # | Thème | Résultats clés |
|---|-------|----------------|
| 1 | Morceaux populaires | *Sweater Weather* est le plus populaire (score 89). Tempo et durée n'influencent pas la popularité. |
| 2 | Genres musicaux | Le pop domine le dataset. Les genres hybrides ont de meilleures moyennes de popularité. |
| 3 | Artistes | Tom Odell et The Neighbourhood ont les meilleures moyennes. Volume de production ≠ popularité. |
| 4 | Tendances temporelles | La popularité augmente avec les années ; les morceaux post-2015 ont des scores plus élevés. |
| 5 | Features musicales vs popularité | Aucune caractéristique musicale ne prédit la popularité (corrélations proches de 0). |
| 6 | Playlists | Les morceaux du top 25% ont légèrement plus d'énergie et de danceabilité. |
| 7 | Artistes & genres | La majorité des artistes restent dans un seul genre musical. |
| 8 | Profil d'un morceau populaire | Pop, fort volume, produit électroniquement, peu acoustique. |

### Partie 2 : Visualisations

- Histogrammes / KDE des caractéristiques musicales
- Boxplot : popularité par genre
- Scatter plot : durée vs popularité
- Bar chart : top 15 artistes par popularité moyenne
- Line plot : évolution temporelle de la popularité
- Boxplot : distribution du tempo par genre
- Heatmap : corrélations entre caractéristiques (énergie ↔ loudness, énergie ↔ acousticness inversée)
- Scatter + Boxplot : morceaux avec valeurs extrêmes

---

## Technologies utilisées

- Python 3
- [pandas](https://pandas.pydata.org/) — manipulation de données
- [numpy](https://numpy.org/) — calcul numérique
- [matplotlib](https://matplotlib.org/) — visualisation
- [seaborn](https://seaborn.pydata.org/) — visualisation statistique
- [scipy](https://scipy.org/) — statistiques avancées
- Jupyter Notebook
