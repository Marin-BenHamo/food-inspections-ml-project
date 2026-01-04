# Chicago Food Inspections – Predicting Inspection Failure

**Student:** Marin Ben-Hamo  
**Course:** Advanced Topics in Machine Learning  
**Instructor:** Prof. Chen Haggag  

---

## 🎯 Project Goal
The objective of this project is to predict whether a food establishment inspection will result in a **Fail** outcome using supervised machine learning classification techniques.  
In addition, unsupervised learning methods are applied to identify patterns, clusters, and anomalous inspection behaviors within the data.

---

## 📊 Dataset
**Source:** Chicago Food Inspections Dataset (data.gov)

- The original CSV dataset is very large and therefore not stored in the repository.
- Data is loaded dynamically at runtime using the **Socrata Open Data API**.
- To ensure reproducibility, the dataset was limited to **300,554 records**.
- A deterministic ordering was applied using `inspection_date` and `inspection_id`, ensuring a stable and consistent dataset across runs.

**Main Features:**
- Inspection type  
- Risk level  
- Facility type  
- Inspection date  
- Geographic location  
- Inspection result (Pass / Fail)

---

## 🛠️ Methods and Algorithms

### Supervised Learning (Classification)
The following models were implemented and evaluated:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- Neural Network (MLP)  

Models were evaluated using Accuracy, ROC-AUC, Precision, Recall, and threshold optimization, with particular emphasis on detecting failed inspections.

---

### Unsupervised Learning
The following unsupervised techniques were applied:

- K-Means Clustering – identification of structural clusters and patterns  
- DBSCAN – detection of dense regions and anomalous inspections  
- PCA – dimensionality reduction and visual exploration  


## 🚀 Quick Start

Clone the repository:
git clone <repository-url>
cd food-inspections-ml-project

Install dependencies:
pip install -r requirements.txt

Run the main notebook:
jupyter notebook ML_project.ipynb

---

## 📊 Data Availability

Due to the large size of the original CSV dataset, the raw data is not stored in this repository.

Instead, the data is loaded dynamically at runtime directly from the official Chicago Food Inspections dataset hosted on data.gov, using the Socrata Open Data API.

A fixed row limit (300,554 records) and deterministic ordering based on inspection_date and inspection_id were applied to ensure reproducibility.

Dataset source:
[https://data.cityofchicago.org](https://catalog.data.gov/dataset/food-inspections)

---

## 📈 Key Findings

- Risk level and inspection type are among the most influential predictors of inspection failure.
- Threshold selection significantly affects the balance between Precision and Recall.
- Unsupervised learning methods revealed clear structural patterns in inspection behavior.

---

## 🔧 Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🤖 AI Tools Disclosure

This project utilized AI assistance (ChatGPT) for code clarification and documentation refinement, in accordance with the course guidelines.



