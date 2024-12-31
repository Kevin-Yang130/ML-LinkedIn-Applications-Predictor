# LinkedIn Job Postings Analysis and Prediction

---

## Project Overview
This project aims to predict the number of applications a job posting will receive on LinkedIn. By analyzing factors such as location, skills, salary, views, and the presence of remote options, we gain deeper insights into the dynamics of job postings and their popularity.

### Goals:
1. Conduct comprehensive Exploratory Data Analysis (EDA).
2. Build regression models to predict the number of applications per job posting.
3. Identify patterns and key factors contributing to "popular" job postings.

---

## Technologies Used
- **Programming Language**: Python
- **Data Analysis and Manipulation**: Pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn
- **Machine Learning Frameworks**: Scikit-learn
- **Notebook Environment**: Jupyter Notebook

---

## Machine Learning Models
Several regression models were implemented to predict the number of applications. Key models include:

4. **Random Forest Regressor**:
   - Non-linear model leveraging decision trees and averaging to improve prediction accuracy.

5. **Gradient Boosting Regressor**:
   - Combines weak learners sequentially for improved performance.
  
6. **Neural Network**:
   - A computational model inspired by the structure and function of the human brain, consisting of layers of interconnected nodes (neurons) that process and learn from data to solve complex problems

---

## Steps in the Project

### Part 1: Data Loading, Preprocessing, and Feature Engineering
1. **Data Loading**:
   - Loaded the dataset containing job postings with attributes such as location, salary, views, and skills.

2. **Data Cleaning**:
   - Removed unnecessary information and handled missing values.
   - Addressed inconsistencies in data formats.

3. **Feature Engineering**:
   - Extracted new features from existing data (e.g., remote vs. on-site jobs).
   - One-hot encoded categorical variables.

### Part 2: Exploratory Data Analysis (EDA)
- Investigated key trends in job postings:
  - Which locations have the highest number of job postings?
  - Do remote jobs attract more applications?
  - Impact of salary on application numbers.
- Visualized insights using Matplotlib and Seaborn.

### Part 3: Model Implementation and Evaluation
- **Train-Test Split**:
  - Split the dataset into training and testing sets to evaluate model performance.

- **Model Training**:
  - Implemented and tuned multiple regression models using Scikit-learn.

- **Evaluation Metrics**:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R-squared (R²)

---

## Key Insights
1. Remote jobs attract significantly more applications than non-remote jobs
2. The number of views is a critical predictor of job applications across models, with its importance being most pronounced in Random Forest and XGBoost. Visibility drives application numbers
3. Location and company size are key factors influencing applications in XGBoost, with more applications generally seen in popular locations and larger companies. 
4. Skill category plays a limited role in predicting the number of applications
5. The relationship between features and applications is non-linear, which aligns with the strengths of models like Random Forest, XGBoost, and Neural Networks

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/LinkedIn-Job-Predictions.git
   ```
2. Navigate to the project directory:
   ```bash
   cd LinkedIn-Job-Predictions
   ```
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook LinkedIn_Job_Postings_CIS545_Project.ipynb
   ```

---

## Future Work
- Implement more advanced models, such as neural networks, for improved predictions.
- Expand analysis to include temporal trends in job postings.
- Build a web-based visualization dashboard to showcase findings interactively.

---
