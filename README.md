# SAE – CSV Data Pipeline (Python, pandas)

![Status](https://img.shields.io/badge/status-finished-green)
![Made with](https://img.shields.io/badge/made%20with-Python-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## 🎯 Objectif
Mettre en place un pipeline de traitement de données CSV hospitalières :  
lecture → nettoyage → enrichissement → fusion → export d’un fichier final exploitable.  

---

## 🧰 Stack & compétences
- **Langages & libs :** Python 3, `pandas`, `datetime`
- **Compétences :**
  - Lecture et écriture de fichiers CSV
  - Nettoyage et normalisation des données
  - Gestion des valeurs manquantes et doublons
  - Création de colonnes calculées (âge, statut, performance)
  - Documentation et traçabilité via un `journal_des_modifications.txt`

---

## 📂 Organisation du projet
```
sd2-sae-csv-pipeline/
├─ src/
│ └─ saecsvscript.py # script Python principal
├─ data/
│ ├─ raw/ # données brutes
│ │ ├─ hospital_data.csv
│ │ └─ additional_hospital_data.csv
│ └─ processed/ # données nettoyées / finales
│ ├─ hospital_nettoyer.csv
│ ├─ additionnal_hospital_nettoyer.csv
│ └─ donnees_hopital_final.csv
├─ docs/
│ └─ Rapport_sae_csv.pdf # rapport de projet
├─ journal_des_modifications.txt # suivi des modifications
└─ README.md
```

---

## 📜 Méthode
1. Lecture des fichiers CSV avec `pandas.read_csv()`.
2. Normalisation des textes et formats de dates.
3. Traitement des valeurs manquantes.
4. Ajout de colonnes calculées (âge, statut de santé, performance).
5. Fusion des datasets + suppression des doublons.
6. Export d’un fichier CSV final propre.
7. Documentation de toutes les étapes dans `journal_des_modifications.txt`.

---

## 🔎 Résultats clés
- Pipeline reproductible, commenté et structuré.
- Données brutes transformées en un **dataset hospitalier final exploitable**.
- Rapport complet détaillant la méthodologie.

---

## ▶️ Exécution
```bash
# Créer un environnement virtuel (optionnel mais recommandé)
python -m venv .venv
.venv\Scripts\activate  # (Windows)
source .venv/bin/activate  # (Linux/Mac)

# Installer les dépendances
pip install pandas

# Lancer le script
python src/saecsvscript.py
```
