# Sequence Classification for Abbreviation and Long Form Detection

**Overview**
This project involves building a sequence classification model to detect abbreviations (AC) and long forms (LF) in biomedical text. The classification task follows the BIO labelling schema, where each token is assigned one of several labels:
B-AC: Beginning of an abbreviation
B-LF: Beginning of a long form
I-LF: Inside of a long form
B-O or O: Other tokens that are neither abbreviations nor long forms.
The dataset used for this task comes from scientific literature in the biomedical domain (PLOS journal articles) and is labelled according to the BIO format. The sequence classification process is crucial in many applications such as healthcare monitoring, intrusion detection, and natural language processing (NLP) tasks like named entity recognition.

**Dataset**
The dataset used for this project is sourced from the PLOD dataset available on Hugging Face:
Labels: B-O, B-AC, B-LF, I-LF
Maximum Token Sequence Length: 323 tokens
Number of Tokens: 50,000 labelled tokens

**Dataset Files**
PLOD-CW: Filtered version of the original PLOD dataset.
PLOD-filtered: Optional dataset for experimentation, but avoid duplicating data.

You can find the datasets at:
PLOD-CW on Hugging Face
PLOD-filtered on Hugging Face

**Task**
Your task is to build a sequence classification model that can correctly identify abbreviations and long forms within a biomedical text. The model should be trained on the provided dataset and should follow the BIO format to label the tokens. You will:
Train a Sequence Classifier: Using labelled tokens from the PLOD dataset.
BIO Format: Implement the BIO schema to label abbreviations and long forms.
Model Evaluation: Evaluate the model's performance using appropriate classification metrics like accuracy, precision, recall, and F1 score.

**Project Structure**
data/: Directory containing the dataset.
notebooks/: Jupyter notebooks containing the model training, evaluation, and visualizations.
scripts/: Python scripts for preprocessing, training, and inference.
README.md: Overview and instructions for the project.
requirements.txt: Python dependencies required for the project.

**Key Features**
BIO Schema: Implemented to identify abbreviations and long forms in biomedical text.
Sequence Classification: Model trained to classify tokens based on the BIO labels.
Preprocessing: Data cleaning, tokenization, and preparation for sequence classification.
Evaluation: Performance metrics such as precision, recall, F1 score, and confusion matrix are used to evaluate the model.
Visualization: Plots generated to visualize the classification performance.

**Results**
The sequence classifier will be evaluated using key performance metrics, including accuracy, precision, recall, and F1 score. The notebook contains detailed results, visualizations, and explanations of the model's performance.
