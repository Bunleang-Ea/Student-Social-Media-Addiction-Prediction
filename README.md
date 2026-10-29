# Social Media Addiction & Mental Health Analysis

## Project Overview
This repository contains a foundational Exploratory Data Analysis (EDA) and baseline machine learning workflow investigating the impact of social media usage on students' mental health. 

The goal of this project is to establish a quantifiable baseline relationship between daily social media habits (usage hours, conflicts, addiction scores) and overall mental health scores using linear regression and rigorous cross-validation techniques.

## Dataset
The analysis utilizes the **Student Social Media Addiction Analysis Dataset** sourced from [Kaggle](https://www.kaggle.com/datasets/zahranusratt/student-social-media-addiction-analysis-dataset). The dataset includes 705 student records. Key features analyzed include:
* `Avg_Daily_Usage_Hours`: Average daily time spent on social media.
* `Sleep_Hours_Per_Night`: Average hours of sleep.
* `Conflicts_Over_Social_Media`: Frequency of social media-related conflicts.
* `Addicted_Score`: Quantified social media addiction level.
* `Mental_Health_Score`: The target variable for our predictive modeling.

## Methodology
1. **Data Assessment:** Verified data quality by checking for duplicate records and null values (the dataset was clean and complete).
2. **Exploratory Data Analysis (EDA):** Generated correlation matrices and scatter plots to visualize the linear relationships between numeric features (usage hours, sleep, conflicts, addiction score) and the target mental health score.
3. **Baseline Modeling:** Split the data (80/20) and trained a baseline Linear Regression model to predict `Mental_Health_Score`.
4. **Model Evaluation:** Evaluated the model using Mean Absolute Error (MAE) and R-squared (R²). 
5. **Cross-Validation:** Implemented a 5-Fold Cross-Validation (with shuffling) to ensure model stability and rule out ordering bias.

## Key Results
* **Baseline Performance:** The initial linear regression model achieved a Mean Absolute Error (MAE) of 0.27 and an R² of 0.89.
* **Validation:** 5-Fold Cross-Validation confirmed the model's robustness, yielding a mean R² score of 0.8936 with a low standard deviation of 0.0064.

## Technologies Used
* **Python 3**
* **Pandas & NumPy** (Data manipulation and assessment)
* **Matplotlib** (Data visualization)
* **Scikit-Learn** (Linear regression, train-test splitting, and K-Fold cross-validation)

## How to Run
1. Clone this repository.
2. Ensure you have the required libraries installed (`pip install pandas numpy matplotlib scikit-learn`).
3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/zahranusratt/student-social-media-addiction-analysis-dataset) and place the CSV in the appropriate `Data/` directory.
4. Run the Jupyter Notebook to view the EDA and model execution.

## Author
**Ea Bunleang**  
*Data Science and Engineering Undergraduate, Royal University of Phnom Penh*
