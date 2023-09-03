# Thesis: Automated Lesion Segmentation in PET/CT Scans Using UNet-based Models

## Table of Contents

1. [Introduction](#introduction)
2. [Objectives](#objectives)
3. [Dataset](#dataset)
4. [Contributing](#contributing)
5. [Acknowledgments](#acknowledgments)

## Introduction

This repository contains all the code, data, and documentation for my thesis project, which focuses on automated lesion segmentation in PET/CT scans using UNet-based deep learning models. The project aims to improve the accuracy and efficiency of lesion segmentation, thereby aiding in better cancer diagnosis and treatment planning.

## Objectives

1. Develop an automated method for lesion segmentation using the UNet architecture.
2. Evaluate the performance of the model using various metrics.
3. Explore the effects of varying imaging protocols on segmentation accuracy.
4. Evaluate the impact of the size and composition of the training dataset on model performance.

## Dataset

The dataset used for this project was downloaded from [MIDAS Lab](http://www.midaslab.org/autoPET/data/nifti.zip) and is stored in an S3 location. The Zip file was downloaded using a Sagemaker Jupyter Notebook instance and extracted to the S3 location.

**Clinical Data (csv):**  
[Download Clinical Metadata](https://wiki.cancerimagingarchive.net/download/attachments/93258287/Clinical%20Metadata%20FDG%20PET_CT%20Lesions.csv?api=v2)

**File Structure:**

\```
|--- Patient 1
     |--- Study 1
          |--- SUV.nii.gz    (PET image in SUV)
          |--- CTres.nii.gz  (CT image resampled to PET)
          |--- CT.nii.gz     (Original CT image)
          |--- SEG.nii.gz    (Manual annotations of tumor lesions)
          |--- PET.nii.gz    (Original PET image as activity counts)
     |--- Study 2            (Potential 2nd visit of same patient)
          |--- ...
|--- Patient 2
     |--- ...
\```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## Acknowledgments

- Special thanks to MIDAS Lab for providing the dataset.
- Thanks to Bharat Kumar for his guidance.
