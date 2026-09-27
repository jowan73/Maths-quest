MATH QUEST — TERMINALE — VERSION iPHONE / PWA
===============================================

CONTENU
-------
index.html              Jeu
style.css               Direction artistique / interface tactile
game.js                 Moteur de jeu + générateurs de questions
manifest.webmanifest    Installation comme app iPhone
sw.js                   Cache hors ligne
icons/                  Icônes iPhone

CE QUI EST DANS LE JEU
----------------------
• Campagne sur 36 semaines et 13 mondes.
• Fondations Seconde/Première conservées toute l'année.
• Course 30 questions / 9 minutes.
• Dojo infini adaptatif.
• Boss hebdomadaire basé sur les thèmes du contrôle.
• Photo du contrôle depuis l'appareil photo ou Photos.
• OCR facultatif si Internet est disponible + sélection manuelle toujours disponible.
• Difficulté qui augmente avec la semaine et la maîtrise du joueur.
• XP, niveaux, pièces, combos, succès et 5 skins.
• Skin 30/30 légendaire automatiquement débloqué en cas de score parfait.
• Statistiques et maîtrise par thème.
• Sauvegarde locale sur l'appareil.
• Sons arcade facultatifs.
• Cache hors ligne du jeu après le premier chargement.

INSTALLATION SUR iPHONE
-----------------------
Une PWA doit être servie depuis une adresse HTTPS. Ouvrir directement index.html depuis
l'app Fichiers ne permet pas une vraie installation iOS.

1. Publier le contenu de CE DOSSIER sur n'importe quel hébergement statique HTTPS.
   Exemples courants : GitHub Pages, Netlify, Cloudflare Pages, serveur personnel HTTPS.
2. Sur l'iPhone, ouvrir l'adresse obtenue dans SAFARI.
3. Toucher Partager.
4. Choisir « Sur l'écran d'accueil ».
5. Activer « Ouvrir comme app web » si l'option apparaît.
6. Toucher Ajouter.
7. Lancer Math Quest depuis son icône comme une application.

Une fois chargé une première fois, le cœur du jeu est mis en cache et fonctionne hors ligne.
L'analyse OCR d'une photo nécessite Internet ; tout le reste, y compris la sélection manuelle
des thèmes, reste utilisable hors ligne.

TEST SUR ORDINATEUR
-------------------
Depuis ce dossier :

  python3 -m http.server 8000

Puis ouvrir http://localhost:8000 dans un navigateur.

REMARQUE
--------
La progression est enregistrée dans le stockage du navigateur / de la web-app. Effacer les
données de Safari ou supprimer l'app web peut effacer la sauvegarde.
