

1. Initialisation du jeu:
   - Un tableau de rectangles (`rect`) est utilisé pour représenter le corps du serpent.
   - Les coordonnées x et y du serpent sont stockées dans les tableaux `xc` et `yc`.
   - La tête du serpent est représentée par le premier rectangle et est initialement colorée en rouge (`Color.RED`).
   - Un rectangle (`food`) représentant la nourriture est initialisé avec une couleur rouge (`Color.RED`) et est placé aléatoirement sur la scène.

2. Déplacement du serpent:
   - La direction du serpent est contrôlée par les touches directionnelles (W, A, S, D).
   - Le déplacement est effectué dans une boucle de jeu qui s'exécute dans un thread séparé.
   - Le serpent se déplace en ajoutant une nouvelle tête à la position suivante et en supprimant la queue.
   - Si le serpent touche la bordure de la scène ou se croise lui-même, le jeu se termine.

3. Collision avec la nourriture:
   - Si la tête du serpent entre en collision avec la nourriture, la nourriture est déplacée à une nouvelle position aléatoire.
   - Une nouvelle partie du corps est ajoutée au serpent, simulant sa croissance.

4. Affichage graphique:
   - Le programme utilise JavaFX pour créer une interface graphique.
   - La scène contient un panneau (`Pane`) sur lequel les rectangles du serpent et la nourriture sont affichés.
   - Les rectangles du serpent sont déplacés pour représenter le déplacement du serpent.

5. Contrôles utilisateur:
   - Les touches W, A, S, D sont utilisées pour changer la direction du serpent.

6. Fin du jeu:
   - Si le serpent touche la bordure ou se croise lui-même, le jeu se termine, et "GAME OVER" est affiché dans la console.

7. Lancement du jeu:
   - Le jeu est lancé en appelant la méthode `launch(args)` dans la méthode `main`.

