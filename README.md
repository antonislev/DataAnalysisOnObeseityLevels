# DataAnalysisOnObeseityLevels
report on Estimation of Obesity Levels Based On Eating Habits and Physical Condition

**# Estimation of Obesity Levels Based on Eating Habits and Physical Condition

![Project Diagram](docs/overview.png)

## 📖 Περιγραφή Έργου
Αυτό το repository περιέχει την πλήρη ανάλυση του dataset “Estimation of Obesity Levels Based On Eating Habits and Physical Condition” (UCI ML Repo). Μέσα από ένα συνεκτικό pipeline data science, καλύπτουμε:

1. **Data Processing** (Καθαρισμός, Scaling, Encoding, PCA)  
2. **Clustering** (K-Means & DBSCAN σε διατροφικά χαρακτηριστικά)  
3. **Classification** (GaussianNB vs NeuralNet για NObesity κατηγορίες)  
4. **Regression** (Feed-Forward vs Transfer Learning για πρόβλεψη BMI)

Κάθε βήμα συνοδεύεται από κώδικα, metrics και οπτικοποιήσεις ώστε να “αφηγηθεί” μια συνεχή ιστορία (data storytelling).

---

## 📂 Δομή Φακέλων

```text
├── data/  
│   ├── data.csv                     # αρχικό raw dataset  
│   ├── data_clean_step_a.csv        # (α) καθαρισμός  
│   ├── data_normalized_step_b.csv   # (β) κανονικοποίηση & διακριτοποίηση  
│   ├── data_encoded_step_c.csv      # (γ) encoding  
│   ├── data_corr_reduced_step_d.csv # (δ1) drop υψηλής συσχέτισης  
│   └── data_pca_step_d.csv          # (δ2) PCA components  
│  
├── notebooks/  
│   ├── 01_data_processing.ipynb     # Βήματα (α)–(δ) με pandas & scikit-learn  
│   ├── 02_clustering.ipynb          # K-Means, DBSCAN, Elbow, Silhouette, plots  
│   ├── 03_classification.ipynb      # GaussianNB vs MLPClassifier, confusion matrix, ROC-AUC  
│   └── 04_regression.ipynb          # Feed-Forward & Transfer Learning, MAE, RMSE, loss curves  
│  
├── scripts/                         # (προαιρετικά) runnable .py scripts  
│  
├── docs/                            # βοηθητικά διαγράμματα & εικόνες  
│   └── overview.png                 # διάγραμμα pipeline (προαιρετικό)  
│  
├── requirements.txt                 # λίστα Python libraries  
└── README.md                        # αυτή η τεκμηρίωση  
**

Φόρτωση & Εκτέλεση Notebooks

01_data_processing.ipynb

Βήμα (α): Καθαρισμός (drop duplicates, outlier removal με IQR)

Βήμα (β): Κανονικοποίηση (StandardScaler) & Διακριτοποίηση (binning)

Βήμα (γ): Encoding (Ordinal + One-Hot)

Βήμα (δ): Μείωση διαστάσεων (correlation drop & PCA)

02_clustering.ipynb

Επιλογή diet features, scaling, Elbow & Silhouette, K-Means vs DBSCAN, PCA scatter plots

03_classification.ipynb

GaussianNB vs MLPClassifier, metrics (accuracy, precision, recall, f1), confusion matrices, multi-class ROC-AUC

04_regression.ipynb

Feed-Forward regressor vs Transfer Learning regressor, metrics (MAE, MAPE, RMSE), loss curve plots

Αποτελέσματα

Τα notebooks περιέχουν inline οπτικοποιήσεις (boxplots, histograms, scatter, bar charts, heatmaps, ROC curves, loss curves) και αναλυτικά σχόλια.
