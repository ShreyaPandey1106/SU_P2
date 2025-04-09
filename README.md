# Assignment 2
##   Requirements

* Python 3.x
* Libraries (install using `pip install -r requirements.txt`):
    * librosa
    * numpy
    * matplotlib
    * scikit-learn
    * tensorflow or pytorch (if using neural networks)
    * pandas
    * etc. (List all libraries used)

##   Setup

1.  **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2.  **Download the dataset:**

    * Download the "Audio Dataset with 10 Indian Languages" from Kaggle:   [https://www.kaggle.com/datasets/hbchaitanyabharadwaj/audio-dataset-with-10-indian-languages](https://www.kaggle.com/datasets/hbchaitanyabharadwaj/audio-dataset-with-10-indian-languages)
    * Place the dataset in the `data/audio/` directory, organizing it into subdirectories for each language (e.g., `data/audio/hindi/`, `data/audio/tamil/`, `data/audio/bengali/`).

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

##   Usage

###   Task A: MFCC Extraction and Analysis

1.  Run the `task_a.py` script:

    ```bash
    python code/task_a.py
    ```

2.  The script will:

    * Extract MFCCs from the audio files.
    * Generate and save MFCC spectrograms in the `reports/mfcc_spectrograms/` directory.
    * (Optional) Perform statistical analysis and save the results (e.g., to a CSV file).

###   Task B: Language Classification

1.  Run the `task_b.py` script:

    ```bash
    python code/task_b.py
    ```

2.  The script will:

    * Load the extracted MFCC features (or extract them if not already done).
    * Preprocess the data (e.g., normalize, split into train/test sets).
    * Train a language classification model (e.g., SVM, Random Forest, Neural Network).
    * Evaluate the model's performance.
    * Save the model and/or evaluation results.

##   Code Documentation

* `code/task_a.py`:
    * Contains functions for loading audio files, extracting MFCCs using the `librosa` library, generating spectrograms using `matplotlib`, and performing statistical calculations using `numpy`.
    * Key functions: `load_audio()`, `extract_mfccs()`, `visualize_spectrogram()`, `compute_mfcc_statistics()`.
* `code/task_b.py`:
    * Contains functions for loading MFCC features, preprocessing the data using `scikit-learn` (e.g., `StandardScaler`, `train_test_split`), training and evaluating classification models (e.g., `SVM`, `RandomForestClassifier`, `NeuralNetwork`), and saving/loading models.
    * Key functions: `load_mfcc_features()`, `preprocess_data()`, `train_model()`, `evaluate_model()`.
* `code/utils.py`:
    * Contains any utility functions used across both tasks, such as file path handling, data loading/saving, etc.

##   Report

The analysis and results are documented in the `reports/analysis.pdf` file. This report includes:

* Comparison of MFCC spectrograms across different languages.
* Statistical analysis of MFCC features.
* Language classification model performance.
* Discussion of challenges and findings.



