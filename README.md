# Racial Bias Removal for Face Age Progression

This repository is for submitting source code for the Term Project for the AI502 class.

## The baseline
- Paper
[Only a Matter of Style: Age Transformation Using a Style-Based Regression Model](https://arxiv.org/abs/2102.02754):
- Source Code
[yuval-alaluf/SAM: Official Implementation for "Only a Matter of Style: Age Transformation Using a Style-Based Regression Model" (SIGGRAPH 2021) https://arxiv.org/abs/2102.02754 (github.com)](https://github.com/yuval-alaluf/SAM)

## Deep Face
In addition to implementing the baseline paper, this project utilizes Facebook's Deepface. We leverage DeepFace's race classification feature.

[serengil/deepface: A Lightweight Face Recognition and Facial Attribute Analysis (Age, Gender, Emotion and Race) Library for Python (github.com)](https://github.com/serengil/deepface)

## Settings
Due to the different dependencies of Deepface and SAM, we recommend the following method.

1. Create a virtual environment based on Python 3.10 using miniconda.
2. Refer to Deepface's page and install from source.
3. Check the behavior of Deepface.
4. Install the latest version of the packages in SAM's /environment/sam_env.yaml file.

## Modification
Most of the code modifications are in training/coach_aging.py. The MODIFICATION section of that file is where we made our modifications.

## Training
For training, see the readme in the SAM repository. You will need a variety of pretrained models.

## Inference Notebook
Here's a link to the Colab page where you can do Face Age Progression with the model you trained with this source code. You can create an animation and an image file, respectively.

### Generating Animation
https://colab.research.google.com/drive/1Ha9iPGjCp6VZcFyjjwXVz7qjFnh3Uov0?usp=sharing

### Generating images
https://colab.research.google.com/drive/1pjXfgdjT6N0z3BXUAuRn47fjTZXBSe3q?usp=sharing
