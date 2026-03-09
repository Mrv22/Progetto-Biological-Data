BD project: Protein Function Prediction

Project Overview
----------------
This project focuses on protein function prediction using multi-label classification techniques. Three different ontologies are considered:
- CC (Cellular Component)
- MF (Molecular Function)
- BP (Biological Process)

Each ontology is modeled separately, with the final submission combining their predictions.

(The complete folder described below is available in this repository: https://drive.google.com/drive/folders/1kbHzNWWgFJfF5S5Z_24CYH40BTFRHiVe?usp=sharing )

File Structure
--------------
- Training and analysis CC,MF,BP: Script for dataset preprocessing and models evaluation.
- best models: folder containing our best trained models for CC, BP, MF.
- binarizer: folder containing Multi-label binarizers for encoding/decoding labels.
- grafici: Folder with charts to evaluate results and performance curves.
- project_results: Script which uses the best models to produce submission
- submission and submission_with_hierarchy_enforced: Final submission files with predictions,      the second one with a iterative hierarchy enforcement for the GO terms after the prediction.
- models evaluation on test holdout: folder containing the prediction and the results of the cafa evaluation for the test set derived from an holdout of the training set.
- REPORT_BD_group_1: Project report detailing methodology and results.

Usage
-----
1. Preprocessing:
Run `Training and analysis CC,MF,BP` to generate the dataset and repeat our analysis and trials.

2. Model Inference:
Load a trained model and perform predictions using 'Project_results'. Ensure to use the corresponding multi-label binarizer for decoding outputs.

3. Submission:
The final predictions are stored in `submission_with_hierarchy_enforced` and in 'submission' in .tsv extension. The details of the 2 different submission are in the report.


Authors
-------
- Marco Venanzi
- Francesco Bortolozzo
- Beatrice Riello