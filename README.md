# Schizophrenia Detection Using Vision Transformer

## Project Overview
This project uses EEG data. The data is converted into Time-Frequency Representation (TFR) images using the **synchrosqueezing** preprocessing technique to detect schizophrenia using a **Vision Transformer (DeiT)** model. The EEG datasets include Poland, Moscow and Kaggle datasets.

**Data Segmentation:**  
- Poland dataset EEG signals are segmented into **30-second** windows.  
- Moscow dataset EEG signals are segmented into **15-second** windows.  

## Jupyter Notebooks Overview

- **Schizophrenia_preprocessing.ipynb**  
  Generates Time-Frequency Representation (TFR) images for **both Moscow and Poland EEG datasets**.

- **preprocessing_kaggle.ipynb**  
  Generates TFR images **only for the Kaggle EEG dataset**.

- **combine_ch_kaggle.ipynb**  
  Combines TFR images from **19 individual EEG channels** into a single composite image for the Kaggle dataset.

- **Schizophrenia_Final.ipynb**  
  Contains the **model training and evaluation code** using Vision Transformer on the generated TFR images.

## Files Included
- Jupyter notebooks (.ipynb)  

## Data Availability
The generated TFR image files are **not included** in this repository due to their large size. You can generate these images yourself by running the preprocessing notebooks on the raw EEG datasets.

If you need the processed image data directly, please contact the author.

## How to Use
1. Clone the repository to your local machine.  
2. Install the required Python packages (check notebooks for details).  
3. Run the preprocessing notebooks to generate TFR images from the EEG datasets.  
4. Use `combine_ch_kaggle.ipynb` to create combined images for Kaggle dataset channels.  
5. Run `Schizophrenia_Final.ipynb` to train and evaluate the Vision Transformer model.  

## Results
The Vision Transformer model used is **DeiT**, and the preprocessing technique applied is **synchrosqueezing**.

- **Poland Dataset Accuracy:** 96.13%  
- **Moscow Dataset Accuracy:** 96.29%  
- **Kaggle Dataset Accuracy:** 88.40%  

## Author
Melky Sedek  
melkysedek9504@gmail.com
