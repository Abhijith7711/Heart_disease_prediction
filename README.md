### Heart Disease Prediction

Predicting heart disease using machine learning is crucial for **early diagnosis**, enabling timely medical intervention and potentially reducing mortality rates. Machine learning models are capable of analyzing complex patterns in health data, offering more accurate and efficient predictions compared to traditional methods. This technology empowers healthcare providers with actionable insights, supporting **personalized treatment plans** and improving patient outcomes in a **cost-effective manner**.

### Dataset Description

The dataset consists of **303 rows** and **14 columns**, providing information about various health parameters related to heart disease. Each row represents an individual case, and the target column indicates the **presence (1)** or **absence (0)** of heart disease.

### . Insights from EDA

From the exploratory data analysis, the following key relationships and trends were observed:

1. **Gender and Heart Disease**:
   - From the analysis, it was found that **females** are more likely to have heart disease than **males**, contrary to the general trend where men are often considered at higher risk.

2. **Chest Pain Type (cp)**:
   - People with chest pain type `0` (typical angina) are **much less likely** to have heart disease compared to other types of chest pain. This suggests that typical angina may not be a strong indicator of heart disease.

3. **Resting Electrocardiographic Results (restecg)**:
   - Individuals with **restecg values `0` and `1`** are **much more likely** to have heart disease than those with a **restecg value of `2`**, indicating that certain heart conditions may be associated with specific electrocardiographic results.

4. **Exercise-Induced Angina (exang)**:
   - **People with exang = 1** (exercise-induced angina) are **much less likely** to have heart disease, which might suggest that this group has better cardiovascular health or less severe conditions.

5. **Number of Major Vessels (ca)**:
   - Individuals with **ca = 4** (number of major vessels colored by fluoroscopy) show an **astonishingly large number of heart patients**, highlighting that the presence of multiple blocked vessels could indicate severe heart disease.

6. **Slope of the Peak Exercise ST Segment (slope)**:
   - **Slope value `2`** (representing the peak exercise ST segment) causes **more heart pain** compared to **slope values `0` and `1`**, indicating that this feature is a strong indicator of heart-related issues.

7. **Thalassemia (thal)**:
   - **Thalassemia value `2`** is associated with a **high chance** of heart disease, suggesting that this specific type of thalassemia could be a critical factor in heart disease risk.

These insights form a comprehensive understanding of the key factors associated with heart disease, which were crucial in guiding model training and improving prediction accuracy.

### 3. Model Training and Results

Several machine learning models were trained and evaluated to predict heart disease. Below are the models used and their respective accuracy scores:

| **Model**                  | **Accuracy Score** |
|----------------------------|--------------------|
| Logistic Regression        | 77.05%            |
| Naive Bayes                | 78.69%            |
| K-Nearest Neighbors (KNN)  | 77.05%            |
| Decision Tree              | 57.38%            |
| Support Vector Machine (SVM)| 78.69%           |
| Random Forest              | 83.61%            |
| XGBoost                    | 78.69%            |

#### Key Observations:
- **Random Forest** achieved the highest accuracy of **83.61%**, making it the best-performing model in this project.
- Models such as Naive Bayes, Support Vector Machine, and XGBoost also demonstrated competitive accuracy of **78.69%**.
- The Decision Tree model had the lowest accuracy of **57.38%**.

Random Forest was selected as the final model for its superior performance and reliability in predicting heart disease.

