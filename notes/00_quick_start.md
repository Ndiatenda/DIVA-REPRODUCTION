# DIVA Reproduction Quick Start

## Project
Forked repo:

https://github.com/Ndiatenda/DIVA-REPRODUCTION

Original repo:

https://github.com/AMLab-Amsterdam/DIVA

Current purpose:
Reproduce the DIVA rotated-MNIST experiments first, then analyse the latent representations and later introduce structured/dependence-based extensions for PhD work.

## Current Branch

Use:

git checkout baseline-diva

Windows path: C:\Users\raeda\Documents\research\PhD\DIVA-REPRODUCTION

Git Bash Path: ~/Documents/research/PhD/DIVA-REPRODUCTION

Activate environment: source diva_env/Scripts/activate

Check Python Version: python --version 

Python 3.6.8 expected

Check Pytorch: python -c "import torch; print(torch.__version__); print(torch.cuda.is_available())"

1.7.0+cpu
False  Expected 

## Key Installed Versions:

Python: 3.6.8

PyTorch: 1.7.0+cpu

torchvision: 0.8.1+cpu

numpy: 1.19.5

matplotlib: 3.4

seaborn: 0.9.0

scikit-image: 0.14.1

scikit-learn: 0.19.1

Note:
PyTorch 1.0.1 was originally targeted but was not installable easily on this Windows/Python setup. PyTorch 1.7.0+cpu was used for local smoke testing.

## Run Supervised Rotated MNIST Experiment

cd paper_experiments/rotated_mnist/supervised

PYTHONPATH=../../.. python experiment_only_sup_diva.py

Important: run from inside the supervised experiment folder.

Reason:
The script uses old relative paths such as: ../../dataset/

## Dataset

MNIST is downloaded into: paper_experiments/rotated_mnist/dataset/MNIST/

This folder is ignored by Git.

The repo already contains supervised index files: 
paper_experiments/rotated_mnist/dataset/supervised_inds_0.npy

paper_experiments/rotated_mnist/dataset/supervised_inds_1.npy
...
