# Food Inspections – חיזוי כישלון בבדיקות מזון  

**קורס:** נושאים מתקדמים בלמידת מכונה  
**מרצה:** Prof. Chen Haggag  
**סטודנטית:** Marin Ben-Hamo  

---

## 🎯 מטרת הפרויקט
מטרת הפרויקט היא לפתח מודלים של למידת מכונה לצורך חיזוי כישלון (Fail) בבדיקות בטיחות מזון, על סמך מאפייני העסק, סוג הבדיקה, גורמי סיכון ומידע מרחבי וזמני.  
בנוסף, בוצע ניתוח לא־מפוקח (Unsupervised Learning) לצורך זיהוי דפוסים, אשכולות וחריגות בנתונים.

---

## 📊 מאגר הנתונים
**מקור הנתונים:**  
Chicago Food Inspections Dataset (דרך data.gov)

**אופן הטעינה:**  
הנתונים נטענים דינמית בזמן הרצת הקוד באמצעות Socrata API.  
על מנת להבטיח שחזור עקבי של הניסויים, הוגדרה הגבלה קבועה למספר הרשומות (300,554) וכן הוחל סדר דטרמיניסטי על הנתונים באמצעות מיון לפי תאריך הבדיקה ומזהה הרשומה (inspection_date, inspection_id).

---

## 🛠️ שיטות ואלגוריתמים

### למידה מפוקחת (Classification)
- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- Neural Network (MLP)  

המודלים הוערכו באמצעות Accuracy, ROC-AUC, Precision, Recall ואופטימיזציית סף החלטה (Threshold).

---

### למידה לא מפוקחת (Unsupervised Learning)
- K-Means Clustering  
- DBSCAN  
- ניתוח מבוסס PCA לצמצום מימדים והמחשה ויזואלית  

---

## 📁 מבנה הריפוזיטורי
