# # Puissance 4 (Connect Four)

Un jeu de Puissance 4 professionnel avec interface web, effets sonores, suivi des statistiques et modes de jeu contre l'IA ou à deux joueurs.

![Puissance 4](static/images/board.svg)

## Fonctionnalités

- 🎮 **Deux modes de jeu** : Jouez contre l'IA ou contre un ami sur le même ordinateur
- 🎵 **Effets sonores** : Sons pour les pièces qui tombent et pour les victoires/défaites
- 📊 **Suivi des statistiques** : Gardez une trace des victoires et des défaites dans les deux modes de jeu
- 📱 **Interface responsive** : Jouez sur n'importe quel appareil grâce à une interface adaptative
- 💫 **Animations** : Les pièces tombent avec une animation fluide

## Comment jouer

1. Choisissez votre mode de jeu : "vs IA" ou "Deux Joueurs"
2. Pour jouer, cliquez sur la colonne où vous souhaitez placer votre pièce
3. Dans le mode contre l'IA, l'ordinateur jouera automatiquement après votre tour
4. Le premier joueur à aligner 4 pièces horizontalement, verticalement ou en diagonale gagne
5. Consultez les statistiques pour voir vos performances au fil du temps

## Architecture technique

Le projet est construit avec les technologies suivantes :

- **Backend** : Flask (Python)
- **Base de données** : SQLite pour enregistrer les statistiques
- **Frontend** : HTML, CSS, JavaScript
- **Animation et graphiques** : SVG et CSS pour les pièces et le plateau
- **IA** : Algorithme personnalisé écrit en Python

### Structure des fichiers

- `app.py` : Application Flask principale, contient les routes et la logique serveur
- `game_logic.py` : Implémentation des règles et de la logique du jeu
- `models.py` : Modèles de base de données pour les statistiques
- `ai_player.py` : Logique de l'IA pour le mode "vs IA"
- `static/` : Contient les fichiers CSS, images et sons
- `templates/` : Contient les fichiers HTML

## Installation et exécution

1. Assurez-vous d'avoir Python 3.7+ installé
2. Installez les dépendances requises :
   ```
   pip install flask flask-sqlalchemy numpy
   ```
3. Lancez l'application :
   ```
   python server.py
   ```
4. Ouvrez votre navigateur à l'adresse http://localhost:5000

## Personnalisation

- Vous pouvez modifier les couleurs des pièces dans les fichiers SVG
- Ajustez la difficulté de l'IA en modifiant l'algorithme dans `ai_player.py`
- Personnalisez les sons en remplaçant les fichiers dans `static/sounds/`

## Crédits

- Développé avec Flask et SQLAlchemy
- Interface utilisateur inspirée des jeux de plateau classiques
- Son et animations créés spécifiquement pour ce jeu
