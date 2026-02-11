#  Melbourne Housing Price Prediction

This project is a machine learning analysis to predict house prices in Melbourne. As a Statistics student, my goal was to apply **Regression Analysis** techniques and compare different algorithms (Decision Tree vs. Random Forest) on real-world data.

### 📂 Dataset
I used the [Melbourne Housing Snapshot](https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot) dataset from Kaggle.
* **Size:** 13,000+ rows
* **Target Variable:** `Price`

###  What I Did
1.  **Data Cleaning:**
    * Found missing values in `BuildingArea` and `YearBuilt`.
    * Filled missing numerical values with the **Median** to avoid outlier effects.
    * Filled categorical missing values with the **Mode**.
2.  **Exploratory Data Analysis (EDA):**
    * Checked the distribution of prices (Right-skewed).
    * Analyzed correlations (Heatmap) to select the best features.
3.  **Modeling:**
    * **Baseline Model:** Decision Tree Regressor
    * **Improved Model:** Random Forest Regressor

### 📊 Results & Key Findings
Comparing the two models showed that the Random Forest approach significantly reduced the error.

| Model | MAE (Mean Absolute Error) |
|-------|---------------------------|
| Decision Tree | ~$260,000 |
| **Random Forest** | **~$190,000** |

**Main Insight:**
According to the Feature Importance analysis, the most critical factors affecting house prices in Melbourne are **Location (Lattitude/Longitude)** and **Room Count**.

---

##  Türkçe Özet
Bu projede, Melbourne emlak verilerini kullanarak ev fiyatlarını tahmin eden bir makine öğrenmesi modeli geliştirdim.

**Neler Yaptım?**
* Veri setindeki eksik değerleri (Missing Values) istatistiksel yöntemlerle (Medyan/Mod) doldurdum.
* Fiyat dağılımlarını ve değişkenler arasındaki ilişkileri inceledim.
* **Decision Tree** ve **Random Forest** algoritmalarını karşılaştırdım. Random Forest kullanarak hata payını yaklaşık **60.000$ düşürmeyi** başardım.
* Analiz sonucunda, ev fiyatlarını belirleyen en önemli faktörün **Konum** olduğunu verilerle doğruladım.

### Libraries Used
* Python
* Pandas & NumPy
* Scikit-learn
* Seaborn & Matplotlib
