# ISIC-Binary-Classification
Melanoma detection with very small train set.
ISIC Binary Classification 
This project contains two Python notebooks for binary classification of medical images (ISIC dataset) using a pretrained ResNet18 model and Mobile-Net.

Contents
LP-v5.ipynb:

A more advanced notebook featuring stratified subsampling, data augmentation, partial fine-tuning of the last layers of ResNet18, and leakage checks. Achieves a best validation balanced accuracy of 0.9228.

Base_line_resnet18.ipynb:

A simpler baseline notebook with larger subsampling, minimal augmentation, training only the final fully connected layer, and leakage verification. Validation balanced accuracy around 0.923.

Requirements
Python 3.7 or higher
Required packages: torch, torchvision, pandas, numpy, openpyxl, and other standard data science libraries
How to Use
Place the ISIC dataset images and the Excel files train_binary.xlsx, val_binary.xlsx, and test_binary.xlsx in the appropriate directories.

Open the desired notebook:

Use LP-v5.ipynb for the advanced pipeline.
Use Base_line_resnet18.ipynb for the baseline pipeline.
The notebooks will perform stratified subsampling and create smaller Excel files if needed.

The model training runs automatically with the defined settings.

Validation results are shown in the logs, and the best model is saved as a .pth file.

<img width="806" height="364" alt="image" src="https://github.com/user-attachments/assets/f89c525d-45c2-4035-adc3-c9051d764895" />
your files must be as below.

<img width="891" height="364" alt="image" src="https://github.com/user-attachments/assets/833a6855-d967-4520-b012-7119f8a8b498" />

