Exploratory Data Analysis (EDA)
1. Dataset Overview (Descriptive Statistics)

The fetal health dataset contains 2,126 records with 21 numerical features extracted from cardiotocography (CTG) exams. The target variable, fetal_health, has three classes:

1 – Normal

2 – Suspect

3 – Pathological

Descriptive statistics such as mean, median, minimum, maximum, and standard deviation were calculated for all features. These statistics help understand the data spread and central tendency. Most variables show noticeable variation, indicating that they carry useful information for classification.

Key observations from statistics:

Features like baseline value, accelerations, and abnormal short-term variability show meaningful differences across fetal health classes.

Some features have high variance, suggesting the presence of outliers.

All features are numeric, making the dataset suitable for machine learning models.

2. Data Preprocessing
🔹 Missing Values

The dataset contains no missing values, so no imputation techniques were required.

🔹 Duplicate Records

Duplicate rows were checked and removed to avoid bias in model training. Only unique CTG records were retained.

🔹 Outlier Detection

Box plots were used to identify outliers in features such as:

Prolonged decelerations

Abnormal short-term variability

Outliers were not removed blindly because, in medical data, extreme values may represent critical fetal conditions. Therefore, outliers were retained to preserve clinical significance.

🔹 Data Wrangling

Feature names were standardized for consistency.

The target variable was treated as a categorical label.

Data was prepared for visualization and later model training.

3. Data Visualization and Insights
📈 Histograms – Feature Distribution

Insights:

Most fetuses fall under the Normal category.

Accelerations are more frequent in normal cases.

Pathological cases show higher abnormal variability.

📦 Box Plots – Outlier and Class Comparison

Insights:

Pathological cases show wider ranges and more extreme values.

Box plots clearly separate normal and pathological classes.

Some overlap exists between Normal and Suspect classes.

🔗 Scatter Plots – Feature Relationships

Insights:

Lower accelerations combined with higher variability often indicate pathological conditions.

Certain feature combinations help visually separate fetal health classes.

Scatter plots reveal nonlinear relationships, supporting the use of advanced ML models.

4. EDA Summary – Key Insights

The dataset is clean and well-structured, with no missing values.

Feature distributions vary significantly across fetal health classes.

Outliers exist but are clinically meaningful.

Visualizations show clear patterns that support machine learning classification.

The dataset is highly suitable for fetal health prediction models.

✅ Deliverables Covered