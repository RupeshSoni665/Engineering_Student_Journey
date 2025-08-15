# Engineering Student Placement Prediction

## 🌟 Project Overview
The **Engineering Student Placement Prediction** project is a comprehensive machine learning pipeline designed to predict the placement status of engineering students based on a rich set of academic, personal, and extracurricular factors. Leveraging a real-world dataset, this project demonstrates data exploration, preprocessing, model training, and prediction for custom profiles. It applies core data science techniques to the domain of educational and career analytics.

---

## ✨ Features

- **Comprehensive Data Analysis**  
  - Initial data loading and inspection using `.info()`, `.isnull().sum()`
  - Identification of numerical and categorical features

- **Insightful Data Visualization**  
  - Scatter plots, bar charts, pie charts, and box plots  
  - Visual relationships: GPA vs. CTC, Backlogs, Internship Trends, Placement Status

- **Robust Data Preprocessing**  
  - Derived `Total_GPA` from all semester GPAs  
  - Smart handling of missing values (dropping or imputing)  
  - Dropping redundant fields like Student ID, Name, Clubs, Skills  
  - Categorical encoding using LabelEncoder and One-Hot Encoding

- **Multiple ML Models**  
  - Logistic Regression  
  - Decision Tree Classifier  
  - Random Forest Classifier

- **Performance Evaluation**  
  - Accuracy scores  
  - `classification_report`: precision, recall, f1-score

- **Custom Student Prediction**  
  - Input a hypothetical student profile  
  - Output: Placement status (Placed/Not Placed) and probabilities

---

## 💻 Technologies Used

- **Language:** Python 3.x  
- **Libraries:**  
  - pandas, numpy  
  - seaborn, matplotlib  
  - scikit-learn  
  - kagglehub  
- **Environment:** Jupyter Notebook (in VS Code)

---

## 📊 Dataset Information

- **Dataset Name:** Engineering Student Journey  
- **Source:** [KaggleHub](https://www.kaggle.com/datasets/rakeshkapilavai/engineering-student-journey/data)
- **Overview:** Insights into students' academic performance, skills, internships, and final placement

### 🔑 Key Features:

- `Age`: Student's age  
- `Gender`: Gender of the student  
- `Branch`: CSE, ECE, MECH, etc.  
- `Total_GPA`: Derived from 8 semester GPAs  
- `Backlogs`: Number of failed courses  
- `Attendance (%)`: Attendance rate  
- `Internship Done`: Yes/No  
- `Internship Domain`: Domain like Research, Software, etc.  
- `Placement Status`: Target variable  
- `Placement Domain`: Domain of placement  
- `CTC (LPA)`: Annual salary  
- `Alumni Path`: Research, Entrepreneurship, etc.

---

## ⚙️ Setup and Installation


```bash
# 1. Clone the Repository
git clone https://github.com/your_username/Engineering-Student-Placement-Prediction.git
cd Engineering-Student-Placement-Prediction

# 2. Create a Virtual Environment
python -m venv jvenv

# 3. Activate the Virtual Environment
# on windows
jvenv\Scripts\activate
# on bash
source jvenv/bin/activate

# Install Dependencies
pip install pandas numpy seaborn matplotlib scikit-learn kagglehub
```

---

## 📁 Project Structure

```bash
Engineering-Student-Placement-Prediction/
├── journey/
│   ├── jvenv/                  # Python virtual environment
│   ├── Notebooks/
│   │   └── note.ipynb         # Jupyter Notebook with complete workflow
│   └── dataset/
│       └── students.csv       # Dataset file
└── README.md                  # Project documentation
```

---

## 🌱 Future Enhancements

- ✅ Interactive Web Application (Flask/Streamlit)

- ✅ Hyperparameter Tuning (GridSearchCV, RandomizedSearchCV)

- ✅ Cross-Validation (K-Fold)

- ✅ Feature Importance Visualization

- ✅ Model Deployment (Flask + Docker)

- ✅ Data Drift Monitoring

- ✅ Advanced Models (e.g., XGBoost, Neural Networks)
