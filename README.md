# Brain Tumor Segmenter - BTC
The python notebooks contain the code for 3D-MRI data processing, feature extraction and 3D multi-modal segmentation of hetrogenous brain tumor-GLIOMA using Convolution Neural Networks .

## Table of Contents

1. [Overview](#overview)
2. [Getting Started](#getting-started)
    1. [Dependencies](#dependencies)
    2. [Installation](#installation)
3. [Project](#project)
4. [Results](#results)
3. [Author](#author)

## Overview <a name="overview"></a>
In the current project, the 3D volumetric segmentation of heterogeneous brain tumors such as Gliomas- anaplastic
astrocytoma, and Glioblastoma Multiforme (GBM) is performed to extract enhancing tumor (ET), whole tumor
(WT), and tumor core (TC) regions using T1, T2, and FLAIR images

## Getting Started <a name="getting-started"></a>

### Dependencies <a name="dependencies"></a>
* Python 3.×
* Libraries: NumPy, Pandas, Seaborn, Matplotlib, open-cv, Keras, Tensorflow, Nibabel, PyDicom, tqdm, glob

### Installation <a name="installation"></a>

* Datasets: The dataset used in this project is publicly available and can be downloaded from [Kaggle](https://www.kaggle.com/datasets/dschettler8845/brats-2021-task1) or https://www.med.upenn.edu/cbica/brats2020/data.html.

### Project  <a name="project"></a>

Brain tumors are the result of abnormal growth of cells and 
have dismal consequences on the patient’s body. The brain 
tumors are categorized on the pattern of cell development, 
which may be noncancerous in nature and are termed as 
benign, whereas the cancerous one is termed as malignant. 
Benign tumors propagate slowly, which do not spread and 
thus have no afect the associated normal brain parenchyma 
while malignant tumors growth is very rapid and afects 
other parts of brain.
**The algorithm is stated below.**
**Input:** List of images with supporting list of labels.
**Output:** Trained model and predictions.
* **Step1:** Import all the images and labels into python lists.
* **Step2:** Resizing all the images to a size of 256*256.
* **Step3:** Converting all the resized images and supporting labels into NumPy arrays.
* **Step4:** Segregating the dataset into train & test sets and perform one-hot encoding on labels.
* **Step5:** Building the model:
* **Step6:** Compiling model by considering following 
parameters:
**Loss function**=categorical_crossentropy.
**Optimizer**=Adam.
**Performance metrics**=Accuracy.
* **Step7:** Introduce callback functions used for metrics 
optimization.
Tensor Board for measurements and visualizations of 
metrics.
Model Checkpoint for check pointing the model weights.
Reduce Learning Rate (LR) on plateau for reducing the 
learning rate for improving the metrics.
* **Step8:** Test the model and get predictions.

## Results<a name="results"></a>

Training and validation curves for each model is saved in the [**report**]([https://github.com/deepsharma1997/Brain_Tumor_Classifier-BTC/tree/main/report]) folder. The classification report on the testing dataset for each model is also saved in this folder.



## Author<a name="author"></a>
* [Deepanshu Sharma](https://github.com/deepsharma1997)


