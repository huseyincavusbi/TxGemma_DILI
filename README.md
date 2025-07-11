# TxGemma for Drug-Induced Liver Injury (DILI) Prediction

This repository contains a Jupyter Notebook that demonstrates how to use the `google/txgemma-2b-predict` model to predict Drug-Induced Liver Injury (DILI). The process involves generating molecular embeddings from SMILES strings and then training a simple logistic regression classifier on these embeddings to make predictions.

## What This Notebook Does

*   **Loads DILI Data:** Fetches the DILI dataset from the Therapeutics Data Commons (TDC), which contains SMILES strings and their corresponding toxicity classifications.
*   **Generates Molecular Embeddings:** Uses the TxGemma model to convert SMILES strings into meaningful numerical vectors (embeddings) that capture their chemical properties.
*   **Trains a Classifier:** A logistic regression model is trained on the generated embeddings to classify whether a molecule is likely to cause liver injury.
*   **Evaluates Performance:** The model's performance is evaluated using accuracy, precision, recall, F1-score, and a confusion matrix.
*   **Visualizes Embeddings:** Uses t-SNE to project the high-dimensional molecular embeddings into a 2D plot, providing an intuitive visualization of how the model separates toxic from non-toxic molecules.

## Why This is Useful

Drug-Induced Liver Injury is a major cause of drug trial failures. Predicting DILI early can save significant time and resources in drug discovery. This notebook demonstrates a practical application with TXGemma, a large language model fine-tuned specifically for therapeutic tasks to build effective predictive models for critical toxicological endpoints.

## Getting Started

To run this notebook, please ensure you complete the following setup:

1.  **GPU Environment:** For best performance, run this notebook in an environment with GPU support (e.g., Google Colab, Kaggle).

2.  **Model Access:** Before using the model, you must accept its terms and conditions on the Hugging Face model page.
    *   Visit the model card here: **[google/txgemma-2b-predict](https://huggingface.co/google/txgemma-2b-predict)**
    *   Click "Agree and access repository" to accept the license if you haven't already.

3.  **Authentication & Execution:** Authenticate your environment with a Hugging Face access token. Simply run the notebook cells sequentially.

## License

The code in this repository is licensed under the MIT License. See the `LICENSE` file for more details.
