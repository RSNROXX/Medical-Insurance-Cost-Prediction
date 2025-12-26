# 🏥 Medical Insurance Cost Prediction

## 📌 Project Overview
This project applies **Machine Learning** to predict the individual medical costs billed by health insurance. By analyzing demographic and health-related factors—such as age, BMI, smoking status, and region—we can determine how these variables influence insurance charges.

The model is built using **Linear Regression** to establish the relationship between these features and the target variable (charges).

## 📂 Dataset
The dataset used in this project is `insurance.csv`, which contains **1338 records** of beneficiaries. The key features are:

* **`age`**: Age of the primary beneficiary.
* **`sex`**: Gender of the contractor (female/male).
* **`bmi`**: Body mass index (indicator of body fat based on height and weight).
* **`children`**: Number of children covered by the plan.
* **`smoker`**: Smoking status (yes/no).
* **`region`**: Residential area in the US (northeast, northwest, southeast, southwest).
* **`charges`**: Individual medical costs billed by health insurance (Target Variable).

## 🛠 Technologies Used
* **Python**: Core programming language.
* **Pandas & NumPy**: For data manipulation and numerical operations.
* **Matplotlib & Seaborn**: For Data Visualization and correlation heatmaps.
* **Scikit-Learn**: For implementing Linear Regression and evaluating model performance.

## 📊 Key Steps
1.  **Exploratory Data Analysis (EDA):**
    * Visualized distributions of Age, BMI, and Sex.
    * Analyzed the correlation heatmap to identify key drivers of cost (e.g., smoking status has a high correlation with charges).
2.  **Data Preprocessing:**
    * Converted categorical columns (`sex`, `smoker`, `region`) into numerical values using mapping.
    * Checked for missing values (none found).
3.  **Model Training:**
    * Split the data: 80% Training, 20% Testing.
    * Trained a **Linear Regression** model.
4.  **Evaluation:**
    * Achieved an **R² Score** of **~0.75** (75%) on both training and testing data, indicating a balanced model without overfitting.
5.  **Predictive System:**
    * Built a system where new user data can be input to predict estimated insurance costs.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone <your-repo-link>
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Open the Jupyter Notebook:
    ```bash
    jupyter notebook "Medical Insurance Cost Prediction.ipynb"
    ```
4.  Run the cells to see the analysis and predictions.

## 📈 Results
* **Training Accuracy:** ~74.8%
* **Testing Accuracy:** ~75.6%
* **Key Insight:** Smoking status is the strongest predictor of insurance charges, followed by Age and BMI.
