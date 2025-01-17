# ⚙️ Data Preprocessing Tools  

This repository contains a **Google Colab** notebook showcasing foundational data preprocessing techniques for machine learning. The notebook covers essential steps to clean, transform, and prepare datasets for modeling.  

<a href="https://colab.research.google.com/github/riyagpt0251/01_google_colab/blob/main/copy_of_data_preprocessing_tools.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" style="animation: pulse 1s infinite;"></a>

---

## ✨ Key Features  

### 🛠️ 1. **Importing Libraries**  
Python libraries used include:  
```python
import numpy as np  
import matplotlib.pyplot as plt  
import pandas as pd  
```

### 📄 2. **Importing the Dataset**  
The dataset is loaded and split into independent (`X`) and dependent (`y`) variables:  
```python
dataset = pd.read_csv('Data.csv')  
X = dataset.iloc[:, :-1].values  
y = dataset.iloc[:, -1].values  
```

**Example Output (`X`):**  
```
[['France' 44.0 72000.0]  
 ['Spain' 27.0 48000.0]  
 ['Germany' 30.0 54000.0]  
 ['Spain' 38.0 61000.0]  
 ['Germany' 40.0 nan]  
 ['France' 35.0 58000.0]  
 ['Spain' nan 52000.0]  
 ['France' 48.0 79000.0]  
 ['Germany' 50.0 83000.0]  
 ['France' 37.0 67000.0]]  
```

**Example Output (`y`):**  
```
['No' 'Yes' 'No' 'No' 'Yes' 'Yes' 'No' 'Yes' 'No' 'Yes']  
```

---

### 🚧 3. **Data Preprocessing Steps**  
- **Handling Missing Data**: Identifying and replacing missing values.  
- **Encoding Categorical Data**: Converting text labels into numerical representations for analysis.  
  - Encoding **Independent Variables**.  
  - Encoding **Dependent Variables**.  
- **Splitting the Dataset**: Dividing the dataset into **Training** and **Test** subsets.  
- **Feature Scaling**: Normalizing data to enhance model performance.

---

## 🚀 How to Use  

1. **Open in Google Colab**: Click the animated badge above to launch the notebook.  
2. **Replace Dataset**: Use your dataset by replacing the file path (`Data.csv`).  
3. **Run Cells**: Execute cells step by step to preprocess the data.

---

## 🎯 Highlights  

- Comprehensive **data preprocessing pipeline**.  
- Handles missing values, categorical data, and scaling.  
- Example dataset included for quick testing.  

---

### 🖥️ Animation Note  
The **Colab badge animation** uses a pulsing effect to grab attention. Add this custom animation in your webpage or Markdown styling:  
```css
@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.05); }
  100% { transform: scale(1); }
}
```

