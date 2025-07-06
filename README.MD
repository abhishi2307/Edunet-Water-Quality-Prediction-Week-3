
# 💧 Water Quality Prediction

This repository contains a machine learning project that predicts the **potability** of water using its chemical and physical features. The aim is to classify whether a given water sample is **safe for human consumption** based on real-world parameters.

---

## 🧠 Project Objective

The goal of this project is to:

- Use supervised machine learning techniques to predict water potability (0 = not potable, 1 = potable).
- Understand the influence of various water characteristics such as pH, hardness, chloramines, etc., on water safety.
- Build a robust model using **Random Forest Classifier** and evaluate its performance.

---

## 📁 Dataset Details

- **Source:** [Kaggle - Water Potability Dataset](https://www.kaggle.com/datasets/adityakadiwal/water-potability)
- **Records:** 3,276 rows × 10 columns
- **Target Feature:** `Potability`

### 🧪 Features Description:

| Feature          | Description                                                       |
|------------------|-------------------------------------------------------------------|
| `pH`             | Level of acidity (0–14)                                           |
| `Hardness`       | Measures the calcium and magnesium in ppm                         |
| `Solids`         | Total dissolved solids (TDS) in ppm                               |
| `Chloramines`    | Chlorine used for disinfection, in ppm                            |
| `Sulfate`        | Sulfate concentration in ppm                                      |
| `Conductivity`   | Electrical conductivity of water in μS/cm                         |
| `Organic_carbon` | Organic carbon content in ppm                                     |
| `Trihalomethanes`| By-products of chlorine, measured in μg/L                         |
| `Turbidity`      | Clarity of the water, in NTU                                      |
| `Potability`     | 0 = Not drinkable, 1 = Safe to drink                              |

---

## ⚙️ Workflow

1. **Data Cleaning**
   - Handled missing values using imputation (mean strategy)
   - Removed null rows and unnecessary records

2. **Exploratory Data Analysis (EDA)**
   - Heatmaps to visualize feature correlation
   - Distribution plots for all features
   - Boxplots to detect outliers

3. **Preprocessing**
   - Feature scaling with `StandardScaler`
   - Train-test split (80/20)

4. **Model Building**
   - Model used: `RandomForestClassifier`
   - Evaluation metrics: Accuracy Score, Confusion Matrix

---

## 🔍 Results

- **Model:** Random Forest Classifier
- **Accuracy:** ~87.6%
- **Observations:**
  - pH, Chloramines, and Sulfate showed strong correlation with Potability
  - Feature scaling improved the model's performance
  - Random Forest handled non-linear features effectively

---

## 📊 Visualizations

- ✅ Correlation Matrix using Seaborn heatmap  
- ✅ Histograms for feature distribution  
- ✅ Confusion Matrix for model evaluation  
- ✅ Countplot of potable vs non-potable samples

---

## 🛠 Tech Stack

- **Programming Language:** Python
- **Libraries:**
  - pandas
  - numpy
  - seaborn
  - matplotlib
  - scikit-learn

---

## 💡 Future Enhancements

- Integrate other models: XGBoost, Logistic Regression
- Deploy model as a web app using **Streamlit** or **Flask**
- Implement auto-retraining pipeline with new data
- Add SHAP/LIME for model interpretability

---

## 📌 Requirements

Example dependencies used in this project:

```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## 🧾 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📬 Feedback

If you found this project useful, give it a ⭐ on GitHub!  
Feel free to open issues or contribute pull requests.
