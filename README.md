# Instrument Classification

This **Instrument Classification** project uses Convolutional Neural Networks (CNN) to classify musical instruments from audio data. .wav files are converted into spectrogram images, which serve as input to the CNN classifier. The model achieved a training accuracy of 99% and a validation accuracy of 74%.

## Table of Contents
- [Dataset](#dataset)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Sample Spectrograms](#sample-spectrograms)
- [Contributing](#contributing)
- [License](#license)

## Dataset
We used the [IRMAS dataset](https://zenodo.org/records/1290750#.WzCwSRyxXMU) for instrument recognition in musical audio signals. The dataset includes various instruments and provides labeled audio files (.wav) used for classification.

## Features
- **Data Preprocessing**: Converts .wav audio files into spectrogram images.
- **CNN Model**: A CNN-based classifier that trains on spectrograms to classify instruments.
- **High Accuracy**: Achieved 99% training accuracy and 74% validation accuracy.

## Tech Stack
- **Framework**: Python, Jupyter Notebook
- **Deep Learning**: TensorFlow/Keras (for CNN model)
- **Environment Management**: Conda
- **Data**: IRMAS dataset (converted into spectrograms)

## Installation

### Prerequisites
Ensure you have the following installed:
- [Anaconda](https://www.anaconda.com/products/distribution) for managing the environment.

### Steps
1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/instrument-classification.git
    cd instrument-classification
    ```

2. **Create and activate the Conda environment**:
    ```bash
    conda env create -f environment.yml
    conda activate instrument-classification
    ```

3. **Download the IRMAS dataset**:
    - Download the dataset from [IRMAS on Zenodo](https://zenodo.org/records/1290750#.WzCwSRyxXMU).
    - Place the dataset in the project’s data directory as instructed in the project structure.

4. **Start Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```
    Open `instrument_classification.ipynb` in the Jupyter interface to view and run the code.

## Usage

1. **Data Conversion**: The notebook includes code to convert .wav files into spectrogram images.
2. **Model Training**: Run the provided cells to train the CNN on the spectrograms.
3. **Classification**: The model will classify new spectrograms with the trained CNN.

## Project Structure
    ├── data                   # Folder for the IRMAS dataset
    ├── notebooks              # Jupyter notebooks
    │   └── instrument_classification.ipynb
    ├── models                 # Saved models (if any)
    ├── spectrograms           # Generated spectrogram images
    ├── images                 # Folder for sample spectrogram images
    ├── environment.yml        # Conda environment configuration
    └── README.md              # Project documentation

## Results
- **Training Accuracy**: 99%
- **Validation Accuracy**: 74%
- **Model Performance**: While training accuracy is high, validation accuracy can be improved with further tuning or data augmentation.

## Sample Spectrograms

Below are sample spectrograms used in this project:

### Violin Spectrogram
![Violin Spectrogram](images/violin_spectrogram.png)

### Piano Spectrogram
![Piano Spectrogram](images/piano_spectrogram.png)


These images represent different instruments in the dataset, transformed from audio files to spectrogram format for the CNN model.

## Contributing
1. Fork the repository.
2. Create your branch: `git checkout -b feature/YourFeature`.
3. Commit your changes: `git commit -am 'Add new feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
