# Comparative Results of VGG16 & RESNET50 for a Cell Counting Regression Task

## Contributors
- Amal Alshammary
- Geng Ding
- Elvis Kimara

## Introduction
This repository contains the implementation of a machine learning approach to automate cell counting in medical images. Our project utilizes the IDCIA v2 dataset to train AI models using VGG16 and ResNet50 architectures. We address challenges such as dataset imbalance, limited data size, and image quality variability by applying data augmentation and transfer learning techniques. The goal is to create an efficient and accurate cell-counting AI model.

For an in-depth understanding of our approach, please refer to the project's [paper](link-to-paper).

![Experimental Design](link-to-figure1)

_Figure 1: Overview of the experimental design_

## Getting Started

### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Required Python libraries: `PIL`, `numpy`

### Setup Instructions
1. Download the `IDCIAv2.zip` and `test_images.zip` into the Google Drive folder where you normally run Python projects.
2. Execute the cell containing `!unzip /content/IDCIAv2.zip` in your Jupyter notebook or similar environment.
3. Refresh the directory listing.
4. Rename the extracted folder from `IDCIA v2` to `IDCIAv2`.

### Running the Code
Follow the order of the Jupyter notebook cells, executing each one sequentially. Please note the following:
- **Augmentation Step**: When running the augmentation cell, a new folder named `new_augmented_images` will be created. Do not rerun the augmentation cell multiple times, as this folder will not be automatically deleted, and it will lead to duplication.

## Repository Structure
- `augmentation.py`: Contains the augmentation function that applies various transformations to the images.
- `undersampling.py`: Script for the undersampling algorithm to balance the dataset.
- `model_training.ipynb`: Jupyter notebook with cells to run the experiments.
- `data`: Folder containing the dataset and any additional files needed for running the experiments.

## Models and Training
We use the following models for our experiments:
- VGG16-Based Regression Model
- ResNet50-Based Regression Model

Customized layers and training hyperparameters can be found within the notebook. For details on the training process and model evaluation, refer to the respective sections within the notebook.

## Experimental Results
Results of our experiments can be found in the `results` section of the Jupyter notebook. This includes performance metrics such as MAE and MSE, and visualizations of the model's predictions versus ground truth.

## Contributing
If you wish to contribute to this project, please fork the repository and submit a pull request with your proposed changes.

## Acknowledgments
This project is partially supported by NSF Award No. 2152117. Special thanks to the individuals and institutions that contributed to the data acquisition and project development.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE-file-link) file for details.

## Contact
- Amal Alshammary - amalha@iastate.edu
- Geng Ding - gengding@iastate.edu
- Elvis Kimara - ekimara@iastate.edu
