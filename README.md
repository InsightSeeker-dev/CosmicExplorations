# 🚀 CosmicExplorations - Android Cloud 2025

Projet académique réalisé dans le cadre du module **Android Cloud 2025**. Cette application native démontre une architecture robuste pour explorer les données de la NASA (Astronomy Picture of the Day).

## 🏗 Architecture & Conception
Le projet respecte scrupuleusement les principes de **Clean Architecture** et **Separation of Concerns** demandés :
* **UI Layer** : Jetpack Compose (Single Activity), Navigation Compose, ViewModels.
* **Data Layer** : Repository Pattern isolant les sources de données.
* **Data Mapping** : Séparation stricte des modèles (`ModelDto` ↔ `ModelEntity` ↔ `ModelData` ↔ `ModelUi`) pour respecter les couches.

## 🛠 Stack Technique
* **Langage** : Kotlin
* **Min SDK** : 26 | **Target SDK** : 35
* **UI** : Jetpack Compose & Material 3
* **Persistence** : Room Database (Offline support)
* **Network** : Retrofit / OkHttp (NASA API)
* **Cloud** : Firebase Messaging & Remote Config (via Repository)

## ✨ Fonctionnalités
1.  **Homepage** : Présentation du groupe.
2.  **Explorer (API + BDD)** :
    * Récupération aléatoire d'images astronomiques.
    * Mise en cache local avec timestamp d'insertion.
    * Liste groupée par date (Header/Footer dynamiques).
3.  **Détail** : Vue détaillée de chaque image.
4.  **Notifications** : Intégration Firebase avec configuration à distance de l'UI.

---
*Développé par Dynastie AMOUSSOU & Mosleh Snoussi*
