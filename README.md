#  Explicabilité de l'Algorithme A* — Planification de Trajets

## Description
Ce projet implémente l'algorithme A* sur une grille 10×10 représentant un entrepôt 
logistique, avec 22 obstacles. Il met l'accent sur l'explicabilité — visualisation 
du chemin optimal et interprétation des décisions prises à chaque étape.

##Auteurs
* **Chaymae Yassine**
* **Maroua Sfaoui**
* **Bassma Cheamou El Fihri**
* **Rania Bennani**

---

## Structure du projet
astar-pathfinding/
│
├── astar_entrepot.ipynb     # Notebook principal
├── README.md                # Documentation du projet
└── images/                  # Graphiques générés
    └── chemin_optimal.png

## Instructions d'exécution
1. Cloner le repo ou télécharger le fichier `.ipynb`
2. Ouvrir dans Jupyter Notebook ou Google Colab
3. Exécuter toutes les cellules dans l'ordre

## Contexte et Problématique
Un robot doit transporter des colis du point de départ (0,0) vers le point 
d'arrivée (9,9) en évitant les obstacles (étagères, murs) dans un entrepôt.

## Méthodologie
### 1. Modélisation de l'environnement
- Création d'une grille 10×10 avec 22 obstacles
- Définition des points de départ et d'arrivée
- Visualisation de la carte de l'entrepôt

### 2. Implémentation de l'algorithme A*
- **g** = distance parcourue depuis le départ
- **h** = distance estimée jusqu'à l'arrivée (heuristique de Manhattan)
- **f = g + h** → A* choisit toujours le nœud avec le plus petit f

### 3. Explicabilité des décisions
- Journal détaillé de chaque étape
- Explication des détours effectués pour éviter les obstacles
- Visualisation du chemin optimal avec numérotation des étapes

## Résultats
-  Chemin optimal trouvé en **18 déplacements**
-  **77 nœuds** explorés sur 100
-  Seulement 23% des cases visitées

## Limites
- Grille de taille fixe (10×10)
- Déplacements uniquement horizontaux et verticaux (pas de diagonale)
- Heuristique de Manhattan uniquement

##  Technologies
Python · NumPy · Matplotlib
