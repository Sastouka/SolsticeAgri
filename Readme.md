# 🌿 Solstice Agri

**Solstice Agri** est une application mobile professionnelle "Offline-First" dédiée à la gestion agricole de précision. Elle permet le suivi complet des récoltes, des interventions techniques et l'analyse de rentabilité pour les exploitations fruitières (Fruits rouges, Arboriculture).

![Flutter](https://img.shields.io/badge/Flutter-3.x-blue?style=flat&logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.x-blue?style=flat&logo=dart)
![Platform](https://img.shields.io/badge/Platform-Android-green?style=flat&logo=android)
![License](https://img.shields.io/badge/License-Proprietary-red)

## 🚀 Fonctionnalités Clés

### 🚜 Pour les Techniciens (Terrain)
* **Saisie des Récoltes :** Enregistrement rapide par bloc/parcelle (Poids, Écarts, Effectif).
* **Journal des Travaux :** Suivi des interventions (Irrigation, Fertilisation, Phytosanitaire, Taille).
* **Mode Hors-ligne :** Fonctionne parfaitement sans connexion internet (Base de données locale Hive).
* **Multilingue :** Support complet FR, EN, AR, ES, ZH, HI.

### 👨‍🔬 Pour les Ingénieurs & Gérants
* **Tableau de Bord Analytique :** Graphiques interactifs (Répartition par variété, par bloc).
* **Module Rentabilité :** Calcul automatique de la Marge Nette (Revenus - Coûts Main d'œuvre - Intrants).
* **Gestion des Coûts :** Configuration des prix de vente, coûts unitaires des intrants et salaires.
* **Rapports PDF :** Génération de rapports d'activité professionnels prêts à être imprimés ou partagés.
* **Export Excel :** Export complet des données pour analyse externe.

### 🛠️ Outils Système
* **Sauvegarde/Restauration :** Export complet de la base de données en format JSON.
* **Gestion des Rôles :** Interface adaptée selon le profil (Technicien ou Ingénieur).
* **Thèmes Dynamiques :** Personnalisation de l'interface (Thèmes Fraise, Myrtille, Citron...).

---

## 📱 Captures d'écran

| Login & Menu | Saisie Récolte | Tableau de Bord | Rapport PDF |
|:---:|:---:|:---:|:---:|
| *(Insérer image)* | *(Insérer image)* | *(Insérer image)* | *(Insérer image)* |

---

## 🛠 Stack Technique

* **Framework :** [Flutter](https://flutter.dev/)
* **Langage :** [Dart](https://dart.dev/)
* **Base de données locale :** [Hive](https://pub.dev/packages/hive) (NoSQL, rapide, léger).
* **State Management :** [Provider](https://pub.dev/packages/provider).
* **Graphiques :** [fl_chart](https://pub.dev/packages/fl_chart).
* **PDF & Impression :** [pdf](https://pub.dev/packages/pdf) & [printing](https://pub.dev/packages/printing).
* **Export Excel :** [excel](https://pub.dev/packages/excel).
* **Achats In-App :** [in_app_purchase](https://pub.dev/packages/in_app_purchase) (Google Play Billing).

---

## 📂 Structure du Projet

```text
lib/
├── main.dart               # Point d'entrée de l'application
├── models/                 # Modèles de données (Harvest, Intervention, etc.)
│   ├── harvest_model.dart
│   ├── intervention_model.dart
│   └── ...
├── providers/              # Gestion d'état (Logique métier)
│   ├── harvest_provider.dart
│   ├── theme_provider.dart
│   └── ...
├── screens/                # Interfaces Utilisateur (Vues)
│   ├── home_screen.dart
│   ├── entry_screen.dart
│   ├── dashboard_screen.dart
│   ├── history_screen.dart
│   └── ...
├── services/               # Services externes (DB, PDF, Excel)
│   ├── database_service.dart
│   └── pdf_service.dart
└── utils/                  # Utilitaires & Traductions
    ├── translations.dart
    └── arabic_helper.dart