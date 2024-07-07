# EEG Data Classification Using Deep Learning 🧠🔍

## Project Overview

This project focuses on the analysis of EEG data to classify different cognitive states using advanced deep learning techniques. The dataset used is sourced from the Mental Arithmetic Tasks Dataset available at [PhysioNet](https://physionet.org/content/eegmat/1.0.0/). The data is pre-cleaned and ready for use, allowing us to concentrate on model implementation and evaluation.

## Objectives 🎯

The main objectives of this project are:

1. Load and preprocess the EEG data.
2. Perform Power Spectral Density (PSD) analysis to identify key frequency bands.
3. Implement and evaluate multiple deep learning models for EEG classification.

## Dataset 📊

The dataset consists of EEG recordings from subjects performing mental arithmetic tasks. It includes signals from different cognitive states (rest and task), recorded during the experiment.

- **Download the dataset**: [PhysioNet Mental Arithmetic Tasks Dataset](https://physionet.org/content/eegmat/1.0.0/)
- **Research paper**: [Dataset Description and Research Paper](https://www.mdpi.com/2306-5729/4/1/14)

## Methodology 🧪

### 1. Load the EEG Data 📂

Load the dataset and inspect its structure to understand the available signals and their corresponding labels.

### 2. Power Spectral Density (PSD) Analysis 📈

- Calculate the band-wise PSD for both rest and task states.
- Focus on key frequency bands: Delta (1-4 Hz), Theta (4-8 Hz), Alpha (8-12 Hz), Beta (12-30 Hz), and Gamma (30-100 Hz).
- Compare the PSDs of the two states to identify differences in brain activity patterns.

### 3. Deep Learning Classification 🤖

- Extract relevant features from the PSD analysis.
- Implement binary classification using two different deep learning models: EEGNet and a second model of choice (e.g., TSCeption, ViT, ATCNet, VAE).
- Train and validate the models using the provided dataset.
- Evaluate the models using appropriate metrics (accuracy, precision, recall, F1-score) and discuss the results.

## Results 🏆

The results of the classification models will be evaluated based on their performance in distinguishing between rest and task states. Key findings from the PSD analysis and model evaluations will be summarized and discussed.

## Repository Structure 📁

```plaintext
.
├── data
│   └── subject-info.csv          # CSV file containing EEG data
├── notebooks
│   └── EEG_Classification.ipynb  # Jupyter Notebook with the complete analysis and code
├── models
│   └── eegnet_model.h5           # Trained EEGNet model
├── README.md                     # Project description and instructions
└── requirements.txt              # List of dependencies and libraries
```

## Installation ⚙️

To run this project, you need to have Python and the required libraries installed. You can install the necessary dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Usage 🚀

1. **Clone the repository**:

```bash
git clone https://github.com/yourusername/eeg-classification.git
cd eeg-classification
```

2. **Download the dataset** from [PhysioNet](https://physionet.org/content/eegmat/1.0.0/) and place the CSV file in the `data` directory.

3. **Open the Jupyter Notebook**:

```bash
jupyter notebook notebooks/EEG_Classification.ipynb
```

4. **Run the notebook** to execute the analysis step-by-step.

## Contributing 🤝

Contributions are welcome! If you have suggestions or improvements, please create a pull request or open an issue.

## License 📜

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
