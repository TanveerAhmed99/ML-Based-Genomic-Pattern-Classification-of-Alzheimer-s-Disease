
---

# 🧬 Alzheimer’s Disease Classification Using Gene Expression Data

This project explores the use of **machine learning models** to classify Alzheimer’s disease patients based on **gene expression profiles**. The motivation is to investigate genomic biomarkers that can help with **early diagnosis** of Alzheimer’s Disease (AD).

---

## 📂 Dataset

The dataset consists of high-dimensional **gene expression data** along with metadata (diagnosis labels).

🔗 Dataset: [Google Drive Link](https://drive.google.com/drive/folders/1qnzKwhJXjrOZjX2UT3sqP6URjueT9vGf?usp=sharing)

* **`GSE118553_expression_filtered.csv`** → Filtered expression matrix (genes × samples)
* **`alz_metadata_final.csv`** → Metadata file containing sample IDs and Alzheimer’s/control labels

---

## ⚙️ Workflow

1. **Data Preprocessing**

   * Loaded gene expression matrix and metadata.
   * Merged data to align expression profiles with diagnosis labels.
   * Applied normalization and filtering to handle high-dimensionality.

2. **Train-Test Split**

   * Data was split into training and testing subsets.
   * Stratification ensured balanced Alzheimer’s vs. control samples.

3. **Model Training & Evaluation**
   We implemented the following **machine learning models**:

   * **Logistic Regression**

     * Baseline linear model for classification.

   * **Random Forest Classifier**

     * Ensemble of decision trees.
     * Provides feature importance ranking of genes.

   * **Support Vector Classifier (SVC)**

     * Kernel-based model for complex boundaries.
     * Suitable for high-dimensional gene expression data.

---

## 📈 Outputs

* **Confusion Matrices** → Visualized classification performance.
* **ROC Curves** → Assessed sensitivity vs. specificity.
* **Accuracy Bar Plots** → Compared models visually.
* **Feature Importance Plots (Random Forest)** → Highlighted genes influencing classification.

---

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/USERNAME/Alzheimers-Classification.git
   cd Alzheimers-Classification
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:

   ```bash
   jupyter notebook Alzheimer’s_Disease_Classification.ipynb
   ```

4. Upload the dataset files (or use the provided Google Drive link).

---

## 📌 Requirements

* Python 3.8+
* pandas
* numpy
* scikit-learn
* matplotlib / seaborn

---

## 📜 License

This project is released under the MIT License.

---

