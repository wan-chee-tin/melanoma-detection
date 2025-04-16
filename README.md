## 🧬 Project Overview
Skin cancer is one of the most common types of cancer, and melanoma is its deadliest form. Studies show that when melanoma is detected at an early stage, the chances of successful treatment and long-term survival increase significantly. However, diagnosing melanoma accurately and promptly can be challenging, as its appearance can vary widely, often resembling benign moles or lesions. This project uses metadata from the HAM10000 dataset to train models that can differentiate between benign and malignant skin lesions, offering a valuable tool for medical professionals in early diagnosis and treatment planning.

## 🚀 How to Run
To get this project up and running on your local machine, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/melanoma-detection.git
   cd melanoma-detection
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
3. Download the image data from Kaggle and place the image files in the `data/` directory, or you can use the provided sample images and metadata in the `data/` folder.
- 15 sample images have been included in the `data/` directory for demonstration and testing purposes.
- If you prefer to use the full image dataset, visit the [HAM10000 dataset on Kaggle](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000) and download the images to the `data/` directory.
- The `data/HAM10000_metadata.csv` file is already included in the repository for reference if you prefer to work with the metadata alone.
4. Launch the Jupyter notebook:
   ```bash
   jupyter notebook melanoma_detection.ipynb

## 📊 Dataset
The HAM10000 dataset is used in this project. It includes:
- 10,000 dermatoscopic images
- Metadata such as lesion type, age, gender, and localization

## 🔍 Exploratory Data Analysis
A series of visualizations and statistical analyses were performed:
- Distribution plots for lesion type, confirmation method, gender, and localization
- Age-related visualizations: histograms, boxplots, and subset analysis for melanoma
- Insightful visualizations created using Matplotlib and Seaborn

## 🧹 Data Preprocessing
Key preprocessing steps included:
- Handling duplicates, missing values, and outliers
- Resizing images and constructing accessible image paths
- Labeling for binary classification (malignant vs benign)
- Dropping irrelevant or incomplete rows/columns
- Resampling for class balance
- Splitting into training and test datasets

## 🧠 Modeling
Several ML and DL models were developed and compared:
- Decision Tree
- Random Forest
- Support Vector Machine
- k-Nearest Neighbors
- Convolutional Neural Network

## 📈 Evaluation
- Model performance was evaluated using accuracy, confusion matrix, and AUC-ROC curves
- Comparative analysis was conducted across all models
- Visual AUC-ROC curve comparison for better interpretation
