# Assignment 2
## Question 1: Speech Enhancement

This section contains the code and reports related to the speech enhancement task.

### Code

* `4th part.ipynb`:   This Colab Notebook implements the novel pipeline/algorithmic approach to combine the speaker identification model with the SepFormer model for enhanced speaker separation and speech enhancement. It includes training/fine-tuning and evaluation.
* `Part 1st to 3rd.ipynb`:   This Colab Notebook covers the initial parts of Question 1, including:
    * Downloading and preprocessing the VoxCeleb datasets.
    * Loading and fine-tuning speaker verification models.
    * Creating the multi-speaker scenario dataset.
    * Performing initial speaker separation and enhancement using the SepFormer model.

### Reports

* `Report Question1.pdf`:   This PDF document provides a detailed report on the speech enhancement experiments, including:
    * Experimental setup and methodology.
    * Results of speaker verification model fine-tuning.
    * Evaluation metrics for speech separation and enhancement (SIR, SAR, SDR, PESQ).
    * Analysis of the proposed pipeline's performance.
    * Discussion of observations and conclusions.

## Question 2: MFCC Feature Extraction and Comparative Analysis of Indian Languages

This section contains the code, reports, and visualizations related to the MFCC feature extraction and language analysis task.

### Code

* `Code.ipynb`:   This Colab Notebook contains the Python code for:
    * Extracting MFCC features from audio samples.
    * Generating and visualizing MFCC spectrograms.
    * Implementing a language classification model.

### Reports and Visualizations

* `Detailed Analysis of MFCC Features Reflecting Acoustic Characteristics of Different Languages.pdf`:   This PDF document provides an in-depth analysis of how MFCC features represent the acoustic characteristics of different languages.
* `Potential Challenges in Using MFCCs for Language Differentiation.pdf`:   This PDF document discusses the challenges involved in using MFCCs for language differentiation, such as speaker variability and background noise.
* `Report Question2.pdf`:   This PDF document presents the overall report for Question 2, summarizing the method, analysis, and findings.
* `Result.png`:   This image file contain a visualization of the results, such as classification accuracy or other performance metrics.
* `mfcc comparison.png`: This image file may contain a visual comparison of MFCC spectrograms for different languages.

## Requirements

* Python 3.x
* Colab 
* Libraries (You'll need to install these using `pip`. Specific libraries are detailed within the individual notebooks, but generally include):
    * librosa
    * numpy
    * scipy
    * matplotlib
    * scikit-learn
    * pytorch 


## Setup

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/ShreyaPandey1106/SU_P2
    cd SU_P2
    ```

2.  **Install Dependencies:**

    * It is highly recommended to create a virtual environment to manage project dependencies.
    * Navigate to each question's directory (`question_1/`, `question_2/`) and check the notebooks for specific library requirements. You can install them using `pip`:

        ```bash
        python -m venv venv
        source venv/bin/activate  # On Linux/macOS
        venv\Scripts\activate  # On Windows
        pip install <library_name>
        ```

        Replace `<library_name>` with the name of the library (e.g., `librosa`, `torch`). It's good practice to install the requirements listed within the notebooks themselves to ensure compatibility.





