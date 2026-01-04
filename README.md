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

---

## 📁 Repository Structure
