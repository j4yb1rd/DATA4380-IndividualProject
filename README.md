![](UTA-DataScience-Logo.png)

# Diagnosing Autism using CNNs over the ABIDE database

**One Sentence Summary**
* This repository outlines the construction of a convolutional neural network used to classify patients with autism using functional MRIs gathered at rest (rs-fMRIs); patient data will be gathered from the ABIDE dataset. 

## Overview

* The task is to use several patients’ rs-fMRIs, convert them individually into time series of 48 features using the Harvard-Oxford Cortical Structural Atlas, and train a convolutional neural network to produce a regression result; namely, this result will be a probability of whether each individual patient has Autism Spectrum Disorder (ASD).  
* Summary of the performance achieved: TBD 

### Motivation and Background

* I was assigned this project as part of my undergraduate and graduate research under Dr. Pedro Maia at UTA. It sounded like an interesting project to work on, especially since I also have ASD. 

* Previous works:
  * [Identification of autism spectrum disorder using deep learning and the ABIDE dataset - PubMed](https://pubmed.ncbi.nlm.nih.gov/29034163/)
  * [Disease prediction using graph convolutional networks: Application to Autism Spectrum Disorder and Alzheimer’s disease - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S1361841518303554)
  * [Enhancing studies of the connectome in autism using the autism brain imaging data exchange II | Scientific Data](https://www.nature.com/articles/sdata201710)
* This appears to be a previous work that I plan on extending using several different models. 
## Summary of Workdone

Include only the sections that are relevant an appropriate.

### Data

* Data:
  * Type: NII or NII.GZ files
    * Input: time series for individual brain regions, as outlined in the Preprocessing / Clean-up section
  * Size: ~100 GB, although it is ~100 MB per file
  * Instances (Train, Test, Validation Split): how many data points? Ex: 1000 patients for training, 200 for testing, none for validation

#### Preprocessing / Clean up

* In order to fully process the data, I had to run it through a masker, which is the name Nilearn gives to its class of objects that can transform raw Nifti objects into Numpy arrays.

#### Data Visualization

TBD

### Problem Formulation

* Define:
  * Input / Output
  * Models
    * Describe the different models you tried and why.
  * Loss, Optimizer, other Hyperparameters.

### Training

* Describe the training:
  * How you trained: software and hardware.
  * How did training take.
  * Training curves (loss vs epoch for test/train).
  * How did you decide to stop training.
  * Any difficulties? How did you resolve them?

### Performance Comparison

* Clearly define the key performance metric(s).
* Show/compare results in one table.
* Show one (or few) visualization(s) of results, for example ROC curves.

### Conclusions

* State any conclusions you can infer from your work. Example: LSTM work better than GRU.

### Future Work

* What would be the next thing that you would try.
* What are some other studies that can be done starting from here.

## How to reproduce results

* In this section, provide instructions at least one of the following:
   * Reproduce your results fully, including training.
   * Apply this package to other data. For example, how to use the model you trained.
   * Use this package to perform their own study.
* Also describe what resources to use for this package, if appropirate. For example, point them to Collab and TPUs.

### Overview of files in repository

* Describe the directory structure, if any.
* List all relavent files and describe their role in the package.
* An example:
  * utils.py: various functions that are used in cleaning and visualizing data.
  * preprocess.ipynb: Takes input data in CSV and writes out data frame after cleanup.
  * visualization.ipynb: Creates various visualizations of the data.
  * models.py: Contains functions that build the various models.
  * training-model-1.ipynb: Trains the first model and saves model during training.
  * training-model-2.ipynb: Trains the second model and saves model during training.
  * training-model-3.ipynb: Trains the third model and saves model during training.
  * performance.ipynb: loads multiple trained models and compares results.
  * inference.ipynb: loads a trained model and applies it to test data to create kaggle submission.

* Note that all of these notebooks should contain enough text for someone to understand what is happening.

### Software Setup
* List all of the required packages.
* If not standard, provide or point to instruction for installing the packages.
* Describe how to install your package.

### Data

* Point to where they can download the data.
* Lead them through preprocessing steps, if necessary.

### Training

* Describe how to train the model

#### Performance Evaluation

* Describe how to run the performance evaluation.


## Citations

* Provide any references.






