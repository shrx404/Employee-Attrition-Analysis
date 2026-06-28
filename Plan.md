📋 **Internship Project — Week 2**  
 **Project Title:** Employee Attrition Prediction using Machine Learning  
 **Assigned Date:** \[23/06/2026\] **Submission Date:** \[30/06/2026\]

---

🎯 **Problem Statement**  
 Every company loses employees — but losing the wrong employees at the wrong time costs the business heavily in hiring, training, and lost productivity. HR departments at large companies spend crores every year trying to figure out *who is likely to leave and why* — before it happens. This is called **Employee Attrition Prediction**, and it is one of the most widely used real-world applications of data science in the corporate world today.

Your task is to build a Machine Learning system that predicts whether an employee is likely to leave the company based on factors like job satisfaction, salary, work-life balance, years at the company, and performance ratings.

You will clean and prepare HR data, handle categorical features, train and compare classification models, analyze what actually drives employees to leave, and deliver insights that an HR team could act on immediately.

---

📦 **Dataset — Where to Get It**  
 Go to this link and download the dataset:  
 🔗 [https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

Steps to download:

* Create a free account on [www.kaggle.com](http://www.kaggle.com) (if you don't have one)  
* Search for **"IBM HR Analytics Employee Attrition"**  
* Download the file — it will be a .csv file named **WA\_Fn-UseC\_-HR-Employee-Attrition.csv**  
* Use the full dataset — it has 1,470 rows which is perfectly manageable

---

✅ **Tasks to Complete**  
 Complete all the following tasks in a Jupyter Notebook (.ipynb):

**Task 1 — Data Loading & Exploration**

* Load the CSV file using Pandas  
* Display the first 10 rows  
* Check how many rows and columns are there  
* Identify the target column (**Attrition** — Yes/No)  
* Count how many employees left vs stayed and calculate the attrition rate as a percentage  
* Identify how many columns are numeric vs categorical  
* Write one observation: what do you notice about the attrition rate — is it balanced or imbalanced?

**Task 2 — Data Cleaning & Preprocessing**

* Check for missing/null values and handle them  
* Drop columns that add no value to prediction (e.g., EmployeeNumber, Over18, StandardHours — these are constant or irrelevant)  
* Convert the target column Attrition from Yes/No to 1/0  
* Encode all remaining categorical columns using One-Hot Encoding (e.g., Department, JobRole, MaritalStatus, BusinessTravel)  
* Scale numeric features using StandardScaler

**Task 3 — Exploratory Data Analysis — EDA**

* Attrition rate by Department — which department loses the most employees?  
* Attrition rate by Job Role — which roles have the highest exit rate?  
* Attrition vs Monthly Income — do lower paid employees leave more?  
* Attrition vs Work-Life Balance rating — is there a visible pattern?  
* Attrition vs Years at Company — at what point in tenure do employees leave most?  
* Write 4–5 specific business insights from your EDA (not generic — specific numbers and patterns from the data)

**Task 4 — Model Building & Comparison**

* Split data into training and test sets (80/20)  
* Handle class imbalance using **class\_weight='balanced'** parameter (a simpler approach than SMOTE — good to know both exist)  
* Train the following 3 models:  
  * Logistic Regression (baseline — also the most explainable to HR teams)  
  * Random Forest Classifier  
  * Gradient Boosting Classifier  
* Record all results in a comparison table inside your notebook

**Task 5 — Model Evaluation**

* Evaluate all 3 models using:  
  * Precision, Recall, F1-Score  
  * ROC-AUC Score  
  * Confusion Matrix  
* Identify and clearly state which model performed best and why  
* For the best model: extract **Feature Importance** — which factors matter most in predicting attrition?  
* Rank the top 10 most important features driving employee exit

**Task 6 — Visualization (Minimum 4 charts)**

* Chart 1: Bar chart showing attrition rate by Department and Job Role  
* Chart 2: Box plot comparing Monthly Income of employees who left vs stayed  
* Chart 3: Confusion Matrix heatmap for your best model  
* Chart 4: Horizontal bar chart of Top 10 Feature Importances from your best model  
* Chart 5 (Bonus): ROC Curve comparing all 3 models on one graph

**Task 7 — HR Insights & Business Recommendations**  
 Write a short paragraph (6–10 lines) inside your notebook answering:

* Which 3 factors most strongly predict that an employee will leave?  
* Which department or job role should HR prioritize for retention efforts?  
* Does salary alone explain attrition or are there other stronger factors?  
* Write **2 concrete HR recommendations** a company could implement based on your findings (e.g., specific policy changes, who to target for a retention conversation)  
* What limitation does this model have that an HR team should be aware of before using it?

---

🛠️ **Tools & Libraries to Use**

| Tool | Purpose |
| ----- | ----- |
| Python 3.x | Main programming language |
| Jupyter Notebook / Google Colab | To write and run your code |
| Pandas | Data loading and cleaning |
| Scikit-learn | Preprocessing, models, and evaluation |
| Matplotlib / Seaborn | Charts and visualization |
| NumPy | Numeric operations |

---

📁 **What to Submit**  
 Create a folder named: **EmployeeAttrition\_\[YourName\]**  
 Inside the folder, include:  
 ✅ analysis.ipynb — Your complete Jupyter Notebook with all 7 tasks  
 ✅ HR\_Attrition.csv — The dataset you used  
 ✅ summary.pdf or summary.docx — A 1-page written summary of your findings written as if you are presenting to an HR Director (non-technical language)  
 ✅ charts/ — A folder with all chart images saved as .png

**Submit the entire folder as a ZIP file \+ paste your Google Colab / Notebook link**  
 **Via:** https://docs.google.com/forms/d/e/1FAIpQLSeNV5yk4lUbzEAmVAZo44Q8qXQgDFEIsWtxjS61PraTDMTueQ/viewform?usp=dialog

---

**⚠️ Important Note for the Intern:**  
 The summary this week must be written for a non-technical reader — specifically an HR Director who has never heard the words "Random Forest" or "ROC curve." If your summary cannot be understood by someone outside data science, rewrite it. The ability to translate model results into business language is what separates a data scientist from a data analyst — and it is a skill this week is directly testing.

