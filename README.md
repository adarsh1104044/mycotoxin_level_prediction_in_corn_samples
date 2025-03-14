# mycotoxin_level_prediction_in_corn_samples

XGBoost Model for Vomitoxin Prediction

Project Overview

This project applies XGBoost regression after Principal Component Analysis (PCA) on spectral data to predict vomitoxin (DON) concentration. The model is built using Google Colab and requires Python-based dependencies.

Installation Instructions

1. Clone the Repository (If Using GitHub)

git clone <repository_url>
cd <project_directory>

2. Set Up the Environment

Install the required Python dependencies using the following command:

pip install -r requirements.txt

If requirements.txt is not provided, manually install key dependencies:

pip install numpy pandas matplotlib seaborn scikit-learn xgboost

Running the Code in Google Colab

1. Upload the Notebook

Open Google Colab.

Click Upload and select the .ipynb file.

2. Upload Dataset

If the dataset is stored locally, upload it to Colab using:

from google.colab import files
uploaded = files.upload()

If stored in Google Drive, mount your drive:

from google.colab import drive
drive.mount('/content/drive')

3. Run the Notebook

Execute all cells in sequence to preprocess data, apply PCA, train the XGBoost model, and evaluate performance.

Expected Outputs

Dimensionality Reduction Results (PCA components visualization)

Model Training Logs

Performance Metrics (MAE, RMSE, R²)

Predicted vs. Actual Value Comparisons

Troubleshooting

Ensure all dependencies are installed.

If Google Drive is not mounting, restart the runtime and re-run the mounting commands.

If you encounter memory issues, reduce dataset size or optimize PCA component selection.

