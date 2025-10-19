# AI-Powered-Fraud-Detection
A machine learning project for detecting fraudulent SWIFT transactions using classification models and feature engineering on real-world-style banking data.
## Project Structure
```
AI-Powered-Fraud-Detection/
│
├─ main.ipynb                # Main Jupyter notebook containing the code and analysis
├─ requirements.txt          # List of Python dependencies needed to run the project
├─ data/                     # Folder containing the dataset files
│   ├─ BankA_SWIFT_Training_Dataset_Full.xlsx  # Training dataset
│   └─ BankA_SWIFT_Testing_Dataset_Full.xlsx   # Testing dataset
├─ LICENSE                   # MIT LICENSE
└─ .gitignore
```
## Features

* **Data Loading & Cleaning**: Reads and preprocesses `.xlsx` SWIFT transaction data.
* **Missing Value Handling**: Imputes missing values using forward fill and mean imputation.
* **Class Imbalance Handling**: Addresses imbalance using oversampling (SMOTE).
* **Feature Engineering**: Encodes categorical features (`LabelEncoder`) and scales numerical features (`StandardScaler`).
* **Model Training**: Implements multiple ML classifiers.
* **Hyperparameter Tuning**: Optimizes KNN and Random Forest models using `GridSearchCV`.
* **Model Evaluation**: Assesses models using Accuracy, ROC-AUC, and F1-Score.
* **Model Saving**: Saves the best performing model (`best_model.pkl`) using `joblib`.

## Installation 

1.  **Clone the repository:**
    ```
    git clone https://github.com/venkatvellapalem/AI-Powered-Fraud-Detection.git
    ```
    ```
    cd AI-Powered-Fraud-Detection
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```
    python -m venv venv
    ```
    #### On Windows:
    ```
    .\venv\Scripts\activate
    ```
    #### On macOS/Linux:
    ```
    source venv/bin/activate
    ```

4.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage 

1.  Ensure the dataset files are present in the `data/` folder.
2.  Launch Jupyter Notebook or Jupyter Lab:
   
    ```
    jupyter notebook main.ipynb
    ```
    or
    ```
    jupyter lab main.ipynb
    ```
4.  Run the notebook cells sequentially to execute the analysis and model training.

## Results

The **tuned K-Nearest Neighbors (KNN)** model achieved the best overall performance on the test set:

| Metric                   | Score  |
| :----------------------- | :----- |
| Accuracy                 | ~81%   |
| ROC-AUC                  | ~0.75  |
| F1-Score (Fraud Class 1.0) | ~0.67  |

## License

Distributed under the MIT License. See `LICENSE` for more information

## Authors

* **Venkat Vellapalem**
    * GitHub: [Venkat Vellpalem](https://github.com/venkatvellapalem)
    * LinkedIn: [Venkat Vellapalem](https://linkedin.com/in/venkatvellapalem)
* **Are Imanth**
    * GitHub: [Are Imanth](https://github.com/AreImanth)
    * LinkedIn: [Are Imanth](https://www.linkedin.com/in/imanth-a-45b9642ba/)
