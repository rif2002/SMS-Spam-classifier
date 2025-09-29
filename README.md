# 📱 SMS Spam Classifier  

## 📌 Project Objective  
Build a machine learning model that classifies SMS messages as **Spam** or **Not Spam** in real time.  
The project also includes an interactive **Streamlit web app** where users can input a message and instantly check the classification.  

---

## 📊 Dataset  
- **Source:** [Kaggle SMS Spam Collection Dataset](https://www.kaggle.com/uciml/sms-spam-collection-dataset)  
- **Size:** 5,574 messages labeled as **ham (legit)** or **spam**  

---

## 🔄 Process  

### 🔹 Data Cleaning  
- Removed duplicates and missing values  
- Converted text to lowercase  
- Tokenization, stopword removal, punctuation removal, stemming  

### 🔹 Exploratory Data Analysis (EDA)  
- Visualized **word frequencies** with Word Clouds  
- Used **histograms, pie charts, and heatmaps** for insights  
- Found that spam messages often include terms like *“free”, “text”, “call”*  

### 🔹 Model Building  
- Implemented three **Naïve Bayes classifiers**:  
  - Gaussian NB  
  - Multinomial NB  
  - Bernoulli NB  
- Evaluated models using **Accuracy, Precision, and Confusion Matrix**  

### 🔹 Deployment  
- Developed a **Streamlit GUI** where users can input a message and classify it as Spam / Not Spam  

---

## 📈 Results  

| Model              | Accuracy | Precision |
|---------------------|----------|-----------|
| Bernoulli NB        | 98%      | 0.99      |
| Multinomial NB ✅   | 97%      | **1.0**   |
| Gaussian NB         | 86%      | 0.85      |

👉 **Chosen Model:** Multinomial Naïve Bayes (best trade-off between accuracy & precision)  

---

## 💡 Key Insights  
- Spam messages frequently contain **promotional/fraudulent terms** like *“free”, “text”, “call”*  
- Ham (legit) messages often use **casual words** like *“ok”, “time”, “come”*  
- **Multinomial NB** is the most effective algorithm for text classification in this dataset  

---

## 🚀 Tech Stack  
- **Python**  
- **Pandas, NumPy, Matplotlib, Seaborn** → Data cleaning & visualization  
- **Scikit-learn** → Model building  
- **Streamlit** → User Interface & Deployment  

---

## ✅ Conclusion  
Successfully built an **SMS Spam Classifier** with **97% accuracy and perfect precision** using the **Multinomial Naïve Bayes algorithm**.  
Integrated with a **Streamlit interface** to make the model accessible and user-friendly.  


