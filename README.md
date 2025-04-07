# Information Extraction for Construction Cost Documents

This repository contains code developed as part of a research project focused on the automatic extraction and classification of information from semi-structured construction cost documents, such as public works price lists.

## Project Description

The project aims to classify the cost textual descriptions basing on a 3 hierarchical level data structure, and finally extract relevant fields (e.g., disciplines, systems, and objects) in the construction sector.
These taxonomies are structured in JSON format and represent different levels of classification. The extraction process supports analysis, validation, and potential integration with digital models such as BIM or cost ontologies.
The dynamic prompt is built as explained in the figure:
![Methodology(1)](https://github.com/user-attachments/assets/32f1ac19-7cac-4a99-83cf-e5606e39c60c)


## Features

- Loading and parsing of structured JSON taxonomies;
- Filtering of data by DISCIPLINE, SYSTEM and OBJECT hierarchical level;
- Design of chained prompts.

## How to Use

1. Open the notebook `nome_notebook.ipynb` in Google Colab or Jupyter Notebook
2. Upload the taxonomy file (`CODIFICA_TOTALE.json`) and follow the execution steps
3. Explore filtering, extraction, and evaluation functionalities
4. Optionally, adapt the code to work with your own dataset

## Evaluation Approach

In this project, the evaluation of extraction accuracy is performed manually, by reviewing and correcting the outputs of the model according to the True positive (TP), False Positives (FP), and False Negatives (FN) metrics. Since a formal gold standard was not available, TP, FP, and FN are computed based on these manual corrections.

## Files in the Repository
The dataset used for this study is in Italian language.

- `nome_notebook.ipynb`: main notebook used for data processing and evaluation
- `CODIFICA_TOTALE.json`: hierarchical taxonomy of construction cost classifications
- (add any other relevant files here)

## License

This project is released under the MIT License. See the LICENSE file for details.

## Author

Chiara Gatto 
PhD Student in Building Engineering
Politecnico di Milano, ABC department
