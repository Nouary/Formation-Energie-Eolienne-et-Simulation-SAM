# 🎥 Tutoriels Vidéo de la Formation

Les vidéos explicatives de la formation sont hébergées sur Google Drive en haute définition :

🔗 **Lien du dossier Google Drive :**  
👉 [Accéder aux vidéos de formation](https://drive.google.com/drive/folders/1IvRUfnHec4ANB735b1wp7S9nZpEergbL?usp=sharing)

---

## 📋 Contenu des Vidéos

### 1. `How_to_download_the_data.mp4`
* **Objectif :** Téléchargement pas-à-pas des données météorologiques et de gisement (vent / solaire) depuis la plateforme officielle **PVGIS**.
* **Points abordés :**
  * Sélection des coordonnées géographiques du site d'étude.
  * Choix des bases de données de réanalyse (ERA5 / SARAH / TMY).
  * Exportation des fichiers horaires au format `.csv`.

---

### 2. `prepare_the_data_to_use.mp4`
* **Objectif :** Nettoyage, mise en forme et adaptation des données météorologiques pour leur intégration dans **NREL SAM** (*System Advisor Model*).
* **Points abordés :**
  * Structure des colonnes requises par le module éolien de SAM (vitesse du vent à différentes hauteurs, direction, pression, température).
  * Conversion et enregistrement aux formats compatibles (`.csv` / `.srw`).
  * Test d'importation et validation dans l'interface de SAM.

---

> [!IMPORTANT]
> ### ⏱️ Note essentielle sur la validation et le dépannage (Vidéo 2) :
> * **Validation réussie à 24:10 :** À la minute **24:10** de la vidéo `prepare_the_data_to_use.mp4`, les données préparées sont importées avec succès dans SAM et on a passé a l'etape suivante **sans aucune erreur**.
> * **Comportement attendu :** Si votre jeu de données s'importe et fonctionne du premier coup comme à 24:10, votre fichier est parfaitement configuré et vous pouvez poursuivre directement votre simulation !
> * **Cas d'erreurs (après 24:10) :** Tout ce qui est présenté **après 24:10** correspond à des tests volontaires d'erreurs courantes . Cette partie a été conçue pour vous aider à diagnostiquer et corriger les causes fréquentes de blocage si vous rencontrez un message d'erreur lors de vos manipulations.
