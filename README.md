##  Overview
This project builds a **production-ready machine learning pipeline** to predict smartphone addiction using behavioral data such as screen time, app usage, sleep patterns, and user activity.

It goes beyond basic modeling by implementing **data preprocessing, feature engineering, class balancing, model training, and a Streamlit-based frontend**.

##  Objective
- Predict whether a user is addicted to smartphone usage
- Analyze behavioral patterns affecting addiction
- Deploy a real-time prediction system


##  Dataset Features
- Demographics: Age, Gender  
- Usage Behavior: Screen time, Social media, Gaming, Work/Study  
- Activity Metrics: Notifications, App opens  
- Lifestyle: Sleep hours, Stress level  
- Target: `addicted_label` (0 = Not Addicted, 1 = Addicted)

##  ML Pipeline

### 1. Data Preprocessing
- Removed irrelevant features (IDs)
- Handled missing values
- Encoded categorical variables

### 2. Feature Engineering
- Total Usage Time
- Sleep Deficit

### 3. Handling Imbalance
- Applied **SMOTE** to balance classes

### 4. Model
- Random Forest Classifier

### 5. Evaluation
- Accuracy
- Classification Report
- Confusion Matrix


##  Results
The model effectively captures behavioral patterns and predicts addiction with strong performance after balancing the dataset.


##  Frontend
Built with **Streamlit**:
- User-friendly interface
- Real-time predictions
- Interactive input controls


##  Tech Stack
- Python
- Scikit-learn
- Pandas / NumPy
- Matplotlib
- Imbalanced-learn (SMOTE)
- Streamlit


##  Run Locally

```bash
pip install -r requirements.txt
python smartphone_addiction_pipeline.py
streamlit run app.py
