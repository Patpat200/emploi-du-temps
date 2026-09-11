# 📅 Emploi du Temps Etudiant

![Version](https://img.shields.io/badge/version-1.0.2-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-iOS%20%7C%20Android-lightgrey.svg)
![Built with](https://img.shields.io/badge/built%20with-Expo-000020.svg)

Une application mobile moderne et fluide pour consulter l'emploi du temps. Conçue pour simplifier la vie des étudiants grâce à la synchronisation automatique et aux notifications de changement de cours.

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Aperçu](#aperçu)
- [Stack Technique](#stack-technique)
- [Installation & Démarrage](#installer-lapplication-android)
- [Construction Android (APK)](#générer-lapk)
- [Configuration](#configuration)
- [Contribuer](#contribuer)

---

## Fonctionnalités

* **🔄 Synchronisation Automatique** : Récupère automatiquement les événements depuis les flux ICS de l'université.
* **🔔 Notifications Intelligentes** : Alerte l'étudiant en cas de :
    * Création d'un nouveau cours.
    * Modification (changement de salle ou d'horaire).
    * Annulation de cours.
* **📡 Mode Hors-Ligne** : Consultez votre emploi du temps même sans connexion internet (mise en cache locale).
* **🎨 Design Moderne** : Interface propre et réactive construite avec **NativeWind** (Tailwind CSS).
* **⚙️ Personnalisable** : Choix de l'intervalle de synchronisation et gestion de l'URL ICS via les paramètres.

## Aperçu

| Vue Calendrier | Détails Cours | Paramètres |
|:---:|:---:|:---:|
| <img src="https://files.catbox.moe/q3fipx.jpg" width="250" alt="Vue Calendrier" /> | <img src="https://files.catbox.moe/doaqyt.jpg" width="250" alt="Détails Cours" /> | <img src="https://files.catbox.moe/dixup5.jpg" width="250" alt="Paramètres" /> |

---

## Stack Technique

Ce projet utilise les dernières technologies de l'écosystème React Native :

* **Framework** : [Expo](https://expo.dev) (SDK 52+)
* **Langage** : [TypeScript](https://www.typescriptlang.org/)
* **Style** : [NativeWind](https://www.nativewind.dev/) (Tailwind CSS pour React Native)
* **Routing** : Expo Router (Navigation basée sur les fichiers)
* **Parsing** : Parseur ICS personnalisé optimisé
* **Build** : EAS (Expo Application Services)

---

## Installer l’application (Android)

1. Aller dans les [Releases](https://github.com/Patpat200/emploi-du-temps/releases) puis télécharger l’APK directement sur votre smartphone Android.
2. Exécuter le fichier que vous avez installé.
3. Et suivez les étapes qui seront indiqué.

---

## Générer l'apk

Pour créer un fichier installable (`.apk`) pour Android via EAS Build :

1.  Assurez-vous d'avoir configuré `eas.json` (profil preview).
2.  Lancez la commande :
    ```bash
    npx eas-cli build --platform android --profile preview
    ```
3.  Téléchargez l'APK depuis le lien fourni à la fin du processus.

---

## Configuration

L'application utilise une URL par défaut définie dans `lib/sync-service.ts`.
Chaque utilisateur peut écraser cette URL directement dans l'application via l'onglet **Paramètres** pour afficher son propre emploi du temps.

---

## Contribuer

Les contributions sont les bienvenues !
1.  Forkez le projet.
2.  Créez votre branche de fonctionnalité (`git checkout -b feature/AmazingFeature`).
3.  Commitez vos changements (`git commit -m 'Add some AmazingFeature'`).
4.  Poussez vers la branche (`git push origin feature/AmazingFeature`).
5.  Ouvrez une Pull Request.

---

**Développé avec ♡ pour les étudiants de l'UHA.**
