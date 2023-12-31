# Synthetic Data Generation for Personal Identifiable Information Anonymization in Images
* [Project Report Slides](https://docs.google.com/presentation/d/1FgMGslRymsfXy86kucmnOzR5UuAhNtgn/edit?usp=sharing&ouid=104314772114472744003&rtpof=true&sd=true)

## Repository Introduction
* This is a project aims for generating labeled synthetic human body images to boost the performance of human body segmentation.
* The code is `private` and will currently not be published due to confidentiality agreement with BMW.

## Personal Identifiable Information(PII) Anonymization in Images
We train a human body segmentation model on the training dataset to achive PII Anonymization in images as the following pipeline

![image](https://github.com/yu-chern/synthetic-data-generation-4-pii-anonymization-in-images/blob/main/final_training.png)


## Generate Synthetic Dataset Through SMPL Model Plus Blender System 
* The code is based and modified on [Learning from Synthetic Humans](https://github.com/gulvarol/surreal). 

The below graph shows the pipeline for this synthesis approach.

![image](https://github.com/yu-chern/synthetic-data-generation-4-pii-anonymization-in-images/blob/main/smpl_blender_pipeline.png)


## Generate Synthetic Dataset Using a Self-training Pipeline Plus a Shape-Guided Diffusion Model
* Create synthetic images using [shape-guided diffusion](https://shape-guided-diffusion.github.io/) model applied on pseudo-labeled images. This process follows the following pipeline.

![image](https://github.com/yu-chern/synthetic-data-generation-4-pii-anonymization-in-images/blob/main/pls_diffusion_pipeline.png)


## Acknowledgements
* Prof. Dr. Massimo Fornasier(TUM) -- Supervises and evaluates the master thesis.
* Dr. Maka Karalashvili(BMW) -- Supervises the thesis project; provides unlabeled datasets; cordinates and connects the project with [shape-guided diffusion](https://shape-guided-diffusion.github.io/) by Berkeley.
* Magioglou Vasileios(BMW) -- Provides the training pipeline in self-training-synthesis; supervises the thesis project.
* Seth Dong Huk Park (UC Berkeley) -- Provides the inference code for [shape-guided diffusion](https://shape-guided-diffusion.github.io/).
