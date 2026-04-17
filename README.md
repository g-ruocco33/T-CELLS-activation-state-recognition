# T-Cells-state-recognition

Normalized segmentation pipeline for automatic T-cell activation state classification

This repository contains the code developed for the thesis project **"Normalized segmentation pipeline for automatic T-cell activation state classification"**.

The project focuses on the analysis of microscopy images of T cells and implements a workflow for segmentation, manual annotation support, feature extraction, and automatic classification of T-cell activation state.

## Project overview

The pipeline was designed to support the distinction between different T-cell states, with particular attention to image normalization, cell segmentation, and the extraction of discriminative information for downstream classification tasks.

The project includes analysis related to T-cell classes such as:
- Naive
- Activated
- Exhausted

## Main notebooks

- `User_manual.ipynb`  
  Main notebook containing the principal workflow of the project.

- `Annotazione_Manuale.ipynb`  
  Notebook used for manual annotation and for generating labels useful for training good/bad models.

## Repository structure

```text
T-Cells-state-recognition/
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
├── User_manual.ipynb
├── Annotazione_Manuale.ipynb
└── thesis/
    └── Giovanni Ruocco Thesis.pdf
```

(La struttura effettiva può variare leggermente a seconda dei file che verranno aggiunti in futuro.)

## Data and project folders

During development, the project used a dataset structure including folders such as:

- `Naive`
- `Activated`
- `Exhausted`
- `Annotazioni_manuali`
- `training_per_norm`
- `Statistiche_all_DS`
- `modelli_goodbad`
- `Plot`

These folders are not necessarily included in the public repository, especially when they contain large files, generated outputs, trained models, or non-shareable data.

## Installation

It is recommended to create a virtual environment before installing dependencies.

```bash
git clone https://github.com/YOUR_USERNAME/T-Cells-state-recognition.git
cd T-Cells-state-recognition
pip install -r requirements.txt
```

## Usage

A typical workflow is:

1. Prepare and organize microscopy images.
2. Run the main analysis pipeline from `User_manual.ipynb`.
3. Use `Annotazione_Manuale.ipynb` for manual labeling and annotation-related tasks.
4. Extract relevant features from segmented cells.
5. Train or evaluate models for automatic classification.

## Data availability

The complete dataset is not included in this public repository for size, privacy, and reproducibility reasons.

If needed, a minimal example dataset or a description of the expected folder structure can be provided in an additional `docs/` or `sample_data/` directory.

## Reproducibility notes

The original development environment may include Google Colab and Google Drive paths. Before reuse, users may need to adapt file paths to their own local or cloud environment.

## License and usage

This project is intended for academic, educational, and non-commercial research use only.

You may read, use, and modify the code for non-commercial purposes, provided that appropriate credit is given to the original author (Giovanni Ruocco).

The original copyright and authorship of this work remain with the author.

Commercial use, commercial redistribution, or integration into commercial products or services is not allowed without prior written permission from the author. Any commercial interest in this project should be discussed directly with the author, who reserves the right to participate in or separately license such use.

For full terms, see the `LICENSE` file.
