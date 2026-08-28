# 🧱 Le Mur des Mitsvot — Un jeu de tri inspiré de la Torah

![License](https://img.shields.io/badge/licence-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-e34f26.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-f7df1e.svg)
![Statut](https://img.shields.io/badge/statut-en%20développement-orange.svg)

**Le Mur des Mitsvot** est un jeu de réflexion, de rapidité et de tri sur navigateur web. Inspiré des textes de la Torah, il propose aux joueurs de bâtir un édifice spirituel et éthique en classant les lois bibliques au rythme de leur descente.

Rangez chaque parole avant qu'elle ne touche le sol : déterminez instantanément s'il s'agit d'une prescription (**À FAIRE**) ou d'une interdiction (**À ÉVITER**) pour poser vos pierres et consolider votre édifice.

---

## 🌐 Démo en ligne

👉 **[Jouer au Mur des Mitsvot](https://cyrilhermantin-create.github.io/mur_des_mitsvots/)**
*(actif une fois GitHub Pages activé sur le dépôt — voir la section Installation)*

---

## 🧠 Démarche pédagogique & développement

Ce projet **open source et entièrement gratuit** a été réalisé dans un but purement **pédagogique**. Il vise à rendre l'apprentissage, la découverte et la mémorisation des lois éthiques de la Torah ludiques, dynamiques et accessibles à tous.

Le jeu propose une sélection de **25 commandements universels** axés sur l'éthique, la justice, la solidarité et la sécurité, volontairement choisis pour leur message de paix et de cohésion sociale — à l'exclusion des prescriptions à caractère violent ou pénal présentes ailleurs dans le corpus biblique, écartées par choix éditorial pour ce format grand public.

L'ensemble du code HTML, CSS et JavaScript a été développé en collaboration avec l'assistant d'intelligence artificielle **Claude (Anthropic)**, sur la base du concept de jeu, de la sélection des commandements et de la recherche exégétique conçus par l'auteur.

---

## 📜 Travail d'exégèse & sources textuelles

Les idées originales, le concept du jeu de tri et la sélection des commandements intégrés au gameplay sont le fruit d'un travail d'exégèse mené par l'auteur. Le codex et les textes du jeu s'appuient sur les sources suivantes :
*   **La Bible Zadok Kahn** (référence principale pour le texte de la Torah)
*   **La Bible Crampon**
*   Recherches complémentaires de l'auteur sur les enseignements attribués à Yeshoua

---

## ✍️ Auteur & crédits

*   **Concepteur-auteur et donneur d'ordre :** Cyril HERMANTIN.
*   **Conception des mécaniques de jeu et recherche exégétique :** Cyril HERMANTIN.
*   **Assistance au développement et à la programmation :** Claude (Anthropic)

---

## 🎯 Concept & gameplay

Le jeu repose sur un système d'arcade et de « Time Attack » intellectuel, avec une difficulté croissante par niveaux.

*   **Mécanique centrale :** des paroles de loi descendent une à une du haut de l'écran, selon un compte à rebours qui raccourcit à chaque niveau. Le joueur doit rapidement analyser la nature de la loi :
    *   ⬅️ **À FAIRE (« tu feras ») :** envoyer la parole vers la gauche pour valider une prescription.
    *   ➡️ **À ÉVITER (« tu ne feras pas ») :** envoyer la parole vers la droite pour valider une interdiction.
*   **Progression & score :** chaque bonne réponse ajoute une pierre à votre édifice, augmente votre score (bonus de rapidité et de série) et maintient vos 3 cœurs de vie ❤️❤️❤️. Enchaînez les bonnes réponses pour battre votre record de « meilleure série ».
*   **Paliers de niveau :** franchir un niveau affiche une anecdote « le saviez-vous » liée au dernier commandement rangé, avant de poursuivre à un rythme plus rapide.
*   **Fin de partie :** la partie se termine quand les 3 cœurs sont épuisés. Un écran récapitule le score final, le niveau atteint, la meilleure série et le nombre de pierres posées.
*   **Son :** effets sonores synthétisés, activables/désactivables via le bouton dédié.

---

## 🕹️ Commandes du jeu

### 💻 Sur ordinateur
*   `←` ou `A` : envoyer la parole vers la gauche (**À FAIRE**)
*   `→` ou `D` : envoyer la parole vers la droite (**À ÉVITER**)

### 📱 Sur smartphone
*   Touchez simplement la porte de gauche ou de droite, ou effectuez un glissement de doigt (swipe) directement sur l'écran.

---

## 🛠️ Stack technique

Projet volontairement minimaliste, sans dépendance ni framework, pour une compatibilité maximale :
*   **Structure :** un seul fichier HTML autonome (HTML + CSS + JavaScript)
*   **Logique de jeu :** JavaScript (Vanilla JS) — minuterie de chute (position calculée en continu via `requestAnimationFrame`, pas de moteur physique), calcul des scores et des séries, gestion des vies et des paliers de niveau
*   **Son :** effets synthétisés en direct via la Web Audio API, aucun fichier audio externe
*   **Données :** tableau d'objets JavaScript en mémoire pour les 25 commandements (pas de base de données)
*   **Aucune dépendance externe**, à l'exception des polices Google Fonts (Cinzel, Alegreya)

---

## 🚀 Installation et lancement local

Le projet tient dans **un seul fichier HTML**. Aucun outil de build n'est nécessaire.

### Lancer en local
1. Clonez le dépôt :
   ```bash
   git clone https://github.com/cyrilhermantin-create/mur_des_mitsvots.git
   cd mur_des_mitsvots
   ```
   — ou téléchargez simplement le fichier `index.html` seul.
2. Double-cliquez dessus, ou ouvrez-le depuis votre navigateur (`Fichier → Ouvrir`).

### Publier sur GitHub Pages
1. Le fichier `index.html` étant déjà présent à la racine du dépôt, aucun renommage n'est nécessaire.
2. Dans **Settings → Pages** du dépôt, activez GitHub Pages sur la branche principale (dossier racine `/`).
3. Le jeu devient accessible à l'adresse ci-dessus, installable en « app » sur mobile via *Ajouter à l'écran d'accueil*.

---

## 🤝 Contribution

Les contributions pour enrichir le corpus de commandements, affiner l'équilibrage de la difficulté ou améliorer l'interface sont les bienvenues.

1. Forkez le projet.
2. Créez une branche pour votre fonctionnalité (`git checkout -b feature/ma-fonctionnalite`).
3. Commitez vos changements (`git commit -m "Ajout de ma fonctionnalité"`).
4. Poussez la branche (`git push origin feature/ma-fonctionnalite`).
5. Ouvrez une **Pull Request**.

---

## 📄 Licence

Ce projet est distribué sous licence **MIT** — voir le fichier `LICENSE`. Cela signifie concrètement que vous êtes libre d'utiliser, modifier et redistribuer ce code, y compris à des fins commerciales, à condition de conserver la mention de copyright et le texte de la licence.

Un crédit visible vers ce projet original en cas de réutilisation ou d'adaptation est apprécié, sans être une obligation légale distincte de la licence MIT.
