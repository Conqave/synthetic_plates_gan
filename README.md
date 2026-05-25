# Synthetic Plates GAN

Notebook for generating synthetic license plates with a GAN-based pipeline.

## What this project does

The notebook covers the full workflow for a synthetic license plate project:

- preparing clean and real plate pairs from the UC3M-LP dataset,
- generating pseudo-plates with augmentation,
- defining the Pix2Pix-style GAN architecture,
- pretraining on synthetic data,
- fine-tuning on real data,
- verifying trained checkpoints.

The project was built as a notebook-first workflow and is intended to be run in Jupyter or Google Colab.

## Notebook structure

- `synthetic_plates_gan.ipynb` - main notebook with data preparation, model definition, training, and verification

## Requirements

Recommended Python packages:

- `torch`
- `numpy`
- `pillow`
- `opencv-python`
- `tqdm`

Depending on the notebook environment, you may also need:

- `matplotlib`
- `jupyter`

## How to run

1. Open `synthetic_plates_gan.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
2. Run the cells in order.
3. Make sure the dataset paths match your local environment.
4. If you are using Colab, adjust the `ROOT` paths so they point to the mounted workspace or drive.
5. Run the data preparation cells before training.
6. Run pretraining first, then fine-tuning, and finally the checkpoint verification cells.

## Project goal

The goal of the project is to generate realistic synthetic license plates and use them to support training and evaluation of the GAN pipeline.

