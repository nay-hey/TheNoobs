# Terrain Classification Model

## Overview

This project was developed as part of the Auburn Waves, SOI 2024 competition. The objective was to create a robust model that accurately predicts the terrain type based on input images.

## Dataset

The dataset provided includes:
- **Training Images**: 6201 images available at aum27/mars-terrain
- **Test Images**: 2000 images available at aum27/mars-terrain-test

## Model

We employed the Vision Transformer (ViT) model to achieve the classification. This model was chosen for its effectiveness in handling image data and its ability to capture complex patterns in visual information.

## Project Structure

- **`ViT.ipynb`**: IPython notebook containing code for training the ViT model.
- **`predictions.ipynb`**: IPython notebook for evaluating the model's performance and generating predictions.
- **`Report.pdf`**: Detailed report outlining the project’s objectives, methodology, results, and conclusions.
- **`Contribution.pdf`**: Document detailing the contributions of each team member.
- **`THE NOOBS_submission.csv`**: CSV file with the model's predictions on the test dataset.

## Prerequisites

To run this project, you need to install the following packages:

```bash
pip install transformers datasets torch torchvision accelerate
pip install transformers[torch] accelerate -U
````
## Installation

### Set Up the Environment

1. Clone the repository.
2. Install the required dependencies using the commands provided above.

### Train the Model

1. Execute the training code in `ViT.ipynb` to train the ViT model on the training dataset.
2. Save the trained model.

### Evaluate and Test

1. After training, evaluate the model's performance using the test dataset with the notebook `predictions.ipynb`.
2. Add your model path to the following variable in `predictions.ipynb`:
    ```python
    model_path = 'path_to_your_saved_model'
    ```
3. The results and predictions will be saved in `predictions.csv`.

## Acknowledgments

We would like to thank the Auburn Waves, SOI 2024 organizers for providing the dataset and the opportunity to participate in this competition.
