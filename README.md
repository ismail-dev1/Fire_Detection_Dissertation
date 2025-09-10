# The Generative Spark: Evaluating Synthetically Trained Residual Networks for Real-World Fire Detection
This repository contains the source code, experimental notebooks, and results for my Master's dissertation. The project investigates the effectiveness of using generative AI (Stable Diffusion) versus curated simulations (Syn-Fire) to create synthetic training data for deep learning-based fire detection models.

Project Overview
The primary challenge in creating reliable vision-based fire detectors is the scarcity of diverse, real-world training data. This project tackles this problem by comparing two distinct synthetic data paradigms:

Curated Synthetic Data: Using the high-fidelity, simulation-based Syn-Fire dataset.

Generative Synthetic Data: Creating a novel dataset using the Stable Diffusion 1.5 text-to-image model.

Models based on the ResNet-18 and ResNet-50 architectures are trained on each of these synthetic datasets and then evaluated on the real-world D-Fire dataset to measure their generalization capabilities.

🚀 Getting Started
Prerequisites

Python 3.9+

An NVIDIA GPU with CUDA support is required for training.

All dependencies can be installed via pip.

Installation & Setup

Clone the repository:

git clone [https://github.com/your-username/fire-detection-dissertation.git](https://github.com/your-username/fire-detection-dissertation.git)
cd fire-detection-dissertation

Create a virtual environment (recommended):

python3 -m venv venv
source venv/bin/activate

Install dependencies:

pip install -r requirements.txt

Download the Datasets:
The datasets are too large to be hosted on GitHub. Please download them from the links below and place them in the data/raw/ directory.

Syn-Fire (imgs/masks): (https://drive.google.com/drive/folders/104tuAsNESO3rIPLz5un1Kqi0dgBKa0yM?usp=share_link)

Stable Diffusion (fire/no-fire): (https://drive.google.com/drive/folders/1XEjnvZkDJ18Dupmh6OmevYhV1J24CDQL?usp=share_link)

D-Fire (test set): (https://drive.google.com/drive/folders/1M01D8KzweE5JjQUEQAds0v5Y4zxXUuPR?usp=share_link)

Running the Experiments

The entire workflow, from data preprocessing to training and evaluation, is documented in the Jupyter notebooks located in the notebooks/ directory.

1_synfire_preprocessing.ipynb: Converts the Syn-Fire imgs and masks into a classification dataset.

2_sd_resnet_training_evaluation.ipynb: Trains and evaluates the ResNet models on the Stable Diffusion dataset.

3_synfire_resnet_training_evaluation.ipynb: Trains and evaluates the ResNet models on the preprocessed Syn-Fire dataset.

Results
The key finding of this research is that models trained on the generative Stable Diffusion dataset demonstrated superior generalization performance on the real-world test set compared to those trained on the curated Syn-Fire dataset.

The final performance metrics and figures for all experiments are located in the results/ directory.

🎓 Citation
If you use this work, please cite the dissertation:

Ismail Faizi. (2025). The Generative Spark: Evaluating Synthetically Trained Residual Networks for Real-World Fire Detection. University of Bristol.
