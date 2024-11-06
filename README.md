# Chest X-ray Image Preprocessing Pipeline

## Overview

The **Chest X-ray Image Preprocessing Pipeline** is designed to enhance the quality of chest X-ray images for better performance in machine learning tasks, particularly in detecting pneumonia and COVID-19. The primary goal of this project is to accurately predict the location of lungs in X-ray images using lung masks, thereby removing irrelevant anatomical structures and focusing solely on the lungs.

## Purpose

The main objectives of this project include:

- **Predicting Lung Locations**: Identifying the precise area of the lungs within X-ray images.
- **Image Processing**: Creating processed images that are more suitable for further machine learning tasks.
- **Enhancing Model Performance**: Facilitating the development of models aimed at detecting pneumonia and COVID-19 by providing cleaner images.

## Methodology

This pipeline utilizes the **UNET architecture**, a convolutional neural network (CNN) specifically designed for image segmentation tasks. The UNET model is well-suited for biomedical image segmentation due to its ability to capture context and precise localization.

### Key Features

- **Lung Mask Prediction**: The pipeline predicts lung masks to identify lung areas in X-ray images.
- **Image Processing Options**:
  - Set all non-lung parts of the image to black.
  - Crop images to focus solely on lung regions using the predicted masks.
  - Apply histogram equalization to enhance contrast, potentially bringing out specific features within the lung regions.

### Options Available

1. **Masking Options**:
   - Set non-lung regions to black.
   - Crop images based on predicted lung masks.

2. **Image Enhancement**:
   - Histogram equalization to improve contrast and highlight important features in the lung regions.

## Installation

To set up this project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/jprich1984/Chest_Xray_Image_Preprocessing_Pipeline.git
