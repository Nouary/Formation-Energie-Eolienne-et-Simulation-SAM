# Formation : Énergie Éolienne et Simulation avec SAM (System Advisor Model)

<p align="center">
  <img src="https://img.shields.io/badge/Organisme-Club%20PowerUP%20%7C%20ENSA%20F%C3%A8s-blue?style=for-the-badge" alt="ENSA Fes" />
  <img src="https://img.shields.io/badge/Logiciel-NREL%20SAM-orange?style=for-the-badge&logo=wind" alt="NREL SAM" />
  <img src="https://img.shields.io/badge/Donn%C3%A9es-PVGIS%20%7C%20TMY-green?style=for-the-badge" alt="PVGIS" />
  <img src="https://img.shields.io/badge/Statut-Read--Only%20%2F%20Tous%20droits%20r%C3%A9serv%C3%A9s-red?style=for-the-badge" alt="License" />
</p>

---

## 📖 Présentation Générale

Ce dépôt regroupe l'ensemble des ressources pédagogiques, supports de cours, données météorologiques et fichiers de simulation de la formation technique intitulée **« Énergie Éolienne et Simulation dans SAM »**, animée par **NOUARY Lhoussaine** pour les élèves-ingénieurs du **Club PowerUP** à l'**École Nationale des Sciences Appliquées de Fès (ENSA Fès)** — Université Sidi Mohamed Ben Abdellah (**USMBA**).

L'objectif de cette formation est de guider les participants depuis les fondements physiques et aérodynamiques du vent jusqu'à la modélisation complète, le calepinage et l'analyse technico-économique d'un parc éolien sous **System Advisor Model (NREL SAM)**.

---

## 🎯 Programme de la Formation

La formation est organisée en trois séances complémentaires :

### 🔹 Séance 1 : Fondements Théoriques & Aérodynamique Éolienne
* Importance de l'énergie éolienne dans le mix énergétique marocain et feuille de route de l'AMEE.
* Origine du vent, gradients de pression, régimes de brises et lecture des diagrammes isobares.
* Turbulence atmosphérique et cisaillement vertical du vent (loi de puissance / profil logarithmique).
* Couplage aéro-mécanique et électrotechnique d'une éolienne moderne (pales, multiplicateur, génératrice, transformateur).
* Démonstration rigoureuse de la **Limite théorique de Betz ($16/27 \approx 59,3\%$)** via les équations de Bernoulli et de conservation de la quantité de mouvement.

### 🔹 Séance 2 : Découverte du Laboratoire NREL & Prise en Main de SAM
* Rôle et méthodologies du National Renewable Energy Laboratory (NREL).
* Présentation de l'environnement et des modules de simulation de **System Advisor Model (SAM)**.
* Paramétrage des courbes de puissance de turbines et modèles de sillage (*wake effect*).

### 🔹 Séance 3 : Étude de Cas Pratique & Simulation Complète
* Extraction et traitement des séries temporelles météo depuis la plateforme européenne **PVGIS**.
* Création et mise en forme des fichiers de vent spécifiques à SAM (`.csv` / `.srw`).
* Configuration de la disposition géométrique du parc éolien (*Turbine Layout*).
* Modélisation détaillée des pertes (aérodynamiques, électriques, disponibilité, environnementales).
* Simulation, interprétation des graphiques de productible annuel et analyse économique.

---

## 🎥 Vidéos Explicatives & Tutoriels

Les enregistrements vidéo complets des démonstrations pratiques sont accessibles sur Google Drive :

👉 **[Accéder au dossier Vidéos de Formation (Google Drive)](https://drive.google.com/drive/folders/1IvRUfnHec4ANB735b1wp7S9nZpEergbL?usp=sharing)**

Consultez le dossier [`Videos/README.md`](Videos/README.md) pour le détail de chaque vidéo :
1. **`How_to_download_the_data.mp4`** : Procédure de téléchargement des données horaires sur PVGIS.
2. **`prepare_the_data_to_use.mp4`** : Nettoyage et formatage pour NREL SAM.
   * *Note importante :* L'importation réussit et fonctionne sans erreur à **24:10**. Tout ce qui suit **24:10** traite des tests volontaires d'erreurs pour vous aider en cas de diagnostic !

---

## 🗂️ Structure du Dépôt

```plaintext
├── README.md                                    # Documentation générale de la formation
├── LICENSE                                      # Notice de droits d'auteur (Lecture seule / All Rights Reserved)
├── Descriptive de formation.pdf                 # Programme officiel, syllabus et références de la formation
├── Wind_Energy_By_NOUARY_Lhoussaine.pdf         # Support de présentation détaillé par le formateur
├── Step by step simulation.pptx                 # Guide visuel étape par étape pour SAM
├── presentation wind energy.pdf                 # Diaporama introductif sur les systèmes éoliens
│
├── Videos/                                      # Dossier dédié aux tutoriels vidéo
│   └── README.md                                # Liens Google Drive et guide de dépannage
│
├── PROJECT/                                     # Étude de cas pratique (Site USMBA Fès)
│   ├── EXEMPLE.srw                              # Modèle source SAM
│   ├── Universite sidi mohammed ben abdellah... # Données de vent préparées pour Fès (.csv & .xlsx)
│   └── tmy_34.033_-4.980_2005_2023.csv          # Données climatiques TMY de référence
│
├── weather files/                               # Banques de données de vent multi-sites
│   ├── Tantan.srw / Tantan.csv                  # Fichiers de gisement éolien pour la région de Tan-Tan
│   ├── CA Northern-Ocean.srw                    # Fichier de vent offshore
│   └── CA Southwestren.xlsx                     # Données comparatives
│
├── Articles/                                    # Littérature scientifique de référence
│   ├── Wake models & CFD wake aerodynamics      # Articles sur les modèles de sillage (Jensen, Gaussian, CFD)
│   └── Wind farm layout optimization            # Travaux sur l'optimisation spatiale des parcs éoliens
│
└── resources/                                   # Documents d'accompagnement
    ├── atlas de vent par AMEE.pdf               # Atlas officiel du vent au Maroc (AMEE)
    └── Manuels et guides de dimensionnement
```

---

## 💻 Logiciels & Outils Recommandés

* **System Advisor Model (SAM) :** [Téléchargement NREL SAM](https://sam.nrel.gov/download.html)
* **Base de données PVGIS :** [Plateforme PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/fr/)
* **Global Wind Atlas :** [globalwindatlas.info](https://globalwindatlas.info/en/)

---

## 🔒 Propriété Intellectuelle & Droits d'Auteur

> [!NOTE]
> **Licence d'utilisation (Lecture Seule / Read-Only) :**  
> Ce dépôt est mis à disposition du public pour une consultation **éducative et personnelle**.  
> **Tous droits réservés © 2025-2026 NOUARY Lhoussaine / Club PowerUP - ENSA Fès.**  
> Toute utilisation commerciale, reproduction ou redistribution non autorisée de ces supports sans accord écrit préalable est interdite.
