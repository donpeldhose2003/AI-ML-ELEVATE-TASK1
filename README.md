Titanic Dataset - Data Cleaning & Preprocessing

📌 Objective
This project demonstrates how to clean and prepare raw data for Machine Learning using the Titanic dataset. It focuses on handling missing values, encoding categorical variables, normalizing numerical features, and identifying/removing outliers.

---

 🛠️ Tools & Technologies
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Seaborn / Matplotlib** – Data visualization
- **Scikit-learn** – Preprocessing (scaling, encoding)

---

 Dataset Description
The dataset contains details of Titanic passengers and includes the following features:

- `PassengerId`: Unique ID
- `Survived`: 0 = No, 1 = Yes (target column)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`

---

🔍 Steps Performed

 1. **Data Loading & Exploration**
- Loaded dataset into a Pandas DataFrame
- Used `.info()`, `.describe()`, and `.isnull().sum()` to inspect structure and missing values

 2. **Missing Value Handling**
- Replaced missing `Age` with median
- Filled missing `Embarked` with mode
- Dropped `Cabin` column due to excessive missing values

 3. **Categorical Encoding**
- Converted `Sex` to numeric (male → 0, female → 1)
- Applied One-Hot Encoding on `Embarked` column

 4. **Normalization**
- Standardized `Age` and `Fare` using `StandardScaler` (mean = 0, std = 1)

 5. **Outlier Detection & Removal**
- Visualized `Age` and `Fare` using boxplots
- Removed outliers using Interquartile Range (IQR) method

 6. **Export**
- Saved the cleaned and preprocessed dataset as `titanic_cleaned.csv`

---

 Output
A cleaned, numeric-only dataset with:
- No missing values
- All features ready for use in machine learning models
- Reduced noise/outliers for better prediction performance

---

 Files Included
- `titanic.csv` – Original dataset
- `titanic_cleaned.csv` – Cleaned output file
- `titanic_preprocessing.ipynb` – Colab-compatible notebook
- `README.md` – This documentation file

---

OUTPUT

![Screenshot 2025-06-23 175106](https://github.com/user-attachments/assets/72a7bf38-e765-473c-b26c-22f858a0772c)


![Screenshot 2025-06-23 175124](https://github.com/user-attachments/assets/ff160075-6eda-4a85-8864-a7be0f8f95bb)

![Screenshot 2025-06-23 175222](https://github.com/user-attachments/assets/0436d400-0701-41b0-8f38-3ffdccab6880)
