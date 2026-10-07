# 🎮 Steam Gameplay Taxonomy & Computational Ludology

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B.svg)](https://streamlit.io/)
[![Machine Learning](https://img.shields.io/badge/ML-Stacking--Ensemble-green.svg)](https://scikit-learn.org/)
[![NLP](https://img.shields.io/badge/NLP-BERT--Embeddings-red.svg)](https://sbert.net/)

## 📌 Project Overview
This research project in **computational ludology** explores the deep structure of game design through the lens of **Steam's folksonomy**. By analysing data from more than **126,000 games**, we turn the "wisdom of the crowd" (user tags) into a rigorous **multidimensional ontology**, validated against established academic frameworks.

### ❓ Research Question
> **"How can a noisy user folksonomy be turned into a structured ontology of game mechanics, capable of modelling the evolution of design and the hybridity of genres?"**

---

## 🚀 Key Features

*   **📊 Multidimensional Analysis**: Gameplay is structured along 8 VGMS dimensions (Genre, Mechanics, Theme, Mood, Aesthetics, Perspective, Setting, Players).
*   **🤖 Automated Classification**: A machine learning pipeline built on a **Stacking Classifier** (Random Forest + XGBoost) validates the structure of the tags.
*   **🧠 NLP Semantics**: **BERT** (`all-mpnet-base-v2`) is used to align the social usage of tags with their linguistic meaning.
*   **📈 Design Evolution**: The hierarchy of genres and mechanics is modelled through **Subsumption** and temporal **PMI**.

---

## 🛠️ Installation and Usage

### 1. Installation
```bash
git clone https://github.com/yanis-ghazi/Game-Mechanics-Classification-Steam.git
cd Game-Mechanics-Classification-Steam
pip install -r requirements.txt
```

### 2. Update Pipeline (New Games)
```bash
python scripts/New_Games_Gameplay_Taxonomy_Creation.py
```

---

## 🔬 8-Step Methodology

The project is organised around 8 research notebooks (`analysis/`):

1.  **Exploration** (`1_First_Data_Base_Analysis.ipynb`): Cleaning and frequent pattern mining with **FP-Growth**.
2.  **Taxonomy** (`2_Gameplay_Tag_Taxonomy.ipynb`): Semantic mapping to the **VGMS** standard.
3.  **Networks** (`3_Network_Analysis_Cooccurrence.ipynb`): **Lift** computation and design affinities.
4.  **Clustering** (`4_Folksonomic_Clustering_Analysis.ipynb`): Community detection with the **Louvain algorithm**.
5.  **Comparison** (`5_Expert_vs_Folksonomy_Comparison.ipynb`): The semantic gap between **publishers** and **players**.
6.  **ML** (`6_Machine_Learning_Classification.ipynb`): Validation through multi-label prediction (accuracy ~51%).
7.  **NLP** (`7_NLP_Deep_Learning_Enrichment.ipynb`): Coherence analysis with **BERT** embeddings.
8.  **Ontology** (`8_Ontology_and_Diachronic_Analysis.ipynb`): **Subsumption** hierarchies and temporal analysis.

---

## 📂 Repository Structure

```text
├── analysis/           # Research notebooks (steps 1 to 8)
├── data/               # SQLite databases and CSV exports (Folksonomic_Clusters.csv)
├── docs/               # Detailed documentation and VGMS definitions
├── reports/            # Consistency reports (classification, clustering)
├── scripts/            # Adapted BERT models and production scripts
└── requirements.txt    # Project dependencies
```

---

## 📚 State of the Art

The project builds on reference academic work:


| **Author(s)** | **Title** | **Contribution to the Project** |
| :--- | :--- | :--- |
| **Windleharth et al.** (2016) | *Full Steam Ahead* | VGMS taxonomy (Video Game Metadata Schema). |
| **Elias et al.** (2012) | *Characteristics of Games* | Structural analysis of game systems. |
| **Li & Zhang** (2020) | *Network Analysis on Steam Tags* | Methodology for co-occurrence network analysis. |
| **Adrian et al.** (2015) | *ConTag: Semantic Tag Recommendation* | Inspiration for the semantic recommendation system. |
| **Lu, Park, & Hu** (2010) | *User tags vs expert-assigned terms* | Folksonomy vs experts comparison (Notebook 5). |
| **Lee et al.** (2014) | *Video Game Metadata Schema* | Validation of the classification dimensions. |
| **Sanderson & Croft** (1999) | *Deriving concept hierarchies from text* | Subsumption algorithm for the tag hierarchy. |
| **Hamilton et al.** (2016) | *Diachronic Word Embeddings...* | Measuring semantic drift through PMI. |
| **Hsu** (2006) | *Jacks of all trades...* | Shannon entropy to measure hybridity. |
| **Aarseth et al.** (2003) | *A multidimensional typology of games* | Foundations of the multidimensional classification. |
| **Swink** (2009) | *Game Feel: A Game Designer's Guide* | Definition of mechanics and the gameplay loop. |

---

## 🔗 Links and Documentation
*   **Full Documentation**: [docs/Analysis_Files_Documentation.md](docs/Analysis_Files_Documentation.md)
*   **Ludological Definitions**: [docs/Ludological_Terms_Definitions.md](docs/Ludological_Terms_Definitions.md)
*   **Bibliography**: Our sources are available in our [Zotero library](https://www.zotero.org/groups/6288352/pdr_stearn/library).

---
*Research project "Game Mechanics Classification Steam" - 2025-2026*
