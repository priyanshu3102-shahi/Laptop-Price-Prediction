# 💻 Laptop Price Prediction  

## 📊 Project Overview  
This project aims to build a machine learning model to predict laptop prices in Euros based on their specifications. By analyzing features such as company, screen size, RAM, CPU, GPU, and weight, the project develops regression models to forecast prices accurately.  

---

## 📂 Dataset Overview  
The dataset contains laptop specifications and their corresponding prices in Euros. Each row represents a laptop with its features and price.  

### Columns Description  

| Column Name     | Description                                | Type          |
|-----------------|--------------------------------------------|---------------|
| Company         | Laptop manufacturer                        | Categorical   |
| Product         | Brand and model of the laptop              | Categorical   |
| TypeName        | Type of laptop (Notebook, Ultrabook, etc.) | Categorical   |
| Inches          | Screen size (inches)                       | Numerical     |
| ScreenResolution| Screen resolution (e.g., 1920x1080)        | Categorical   |
| CPU_Company     | CPU manufacturer (Intel, AMD)              | Categorical   |
| CPU_Type        | Type of CPU                                | Categorical   |
| CPU_Frequency   | CPU speed (GHz)                            | Numerical     |
| RAM (GB)        | RAM size (GB)                              | Numerical     |
| Memory          | Storage type and size (HDD/SSD)            | Categorical   |
| GPU_Company     | GPU manufacturer (Nvidia, AMD)             | Categorical   |
| GPU_Type        | Type of GPU                                | Categorical   |
| OpSys           | Operating system                           | Categorical   |
| Weight (kg)     | Laptop weight (kg)                         | Numerical     |
| Price (Euro)    | Target variable: laptop price              | Numerical     |

---

## ⚙️ Project Pipeline  

### **Part 1: Data Ingestion**
- Load dataset into a DataFrame.  
- Check data integrity (rows, columns, dtypes, missing values, duplicates).  

### **Part 2: Exploratory Data Analysis (EDA)**
- **Univariate Analysis:** Explore distributions of Price, Inches, RAM, Weight, CPU_Frequency.  
- **Bivariate Analysis:** Explore relationships between features and Price.  
- **Multivariate Analysis:** Use heatmaps, pair plots for correlations.  

### **Part 3: Data Cleaning**
- Handle missing values.  
- Remove duplicates.  
- Standardize categorical values.  

### **Part 4: Data Preprocessing**
- Encode categorical variables (One-Hot, Label Encoding).  
- Scale numerical features.  
- Handle outliers.  
- Engineer new features (e.g., separate HDD/SSD from Memory).  

### **Part 5: Model Building & Evaluation**
- Split data into train/test sets.  
- Train regression models: Linear Regression, Decision Tree, Random Forest, Gradient Boosting.  
- Hyperparameter tuning with GridSearchCV.  
- Evaluate using R², MSE, RMSE.  
- Select the best model for deployment.  

---

## 🛠️ Tech Stack  
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Environment:** Jupyter Notebook / VS Code  

---

## 📁 Repository Structure  

Laptop-Price-Prediction/<br>
│<br>
├── data/<br>
│   └── laptop_data.csv               # Dataset file <br>
│<br>
├── notebook/<br>
│   └── Laptop_Price_prediction.ipynb       # Data loading and inspection <br>
│                          <br>
└── README.md                   # Python dependencies<br>
