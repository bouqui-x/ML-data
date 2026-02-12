# Salary Prediction Using Machine Learning

A machine learning project that predicts employee salaries based on their experience, test scores, and interview performance using Linear Regression.

## 📋 Project Overview

This project builds a predictive model for an HR department to help determine appropriate salaries for job candidates. The model analyzes three key factors:
- Years of experience
- Written test score
- Personal interview score

## 🎯 Objective

Given historical hiring data, train a Linear Regression model to predict salaries for new candidates based on their qualifications.

## 📊 Dataset

The dataset contains 8 records with the following features:

| Feature | Description |
|---------|-------------|
| experience | Years of work experience (text format) |
| test_score | Written test score (0-10) |
| interview_score | Personal interview score (0-10) |
| salary | Annual salary in USD (target variable) |

**Sample Data:**
```
experience | test_score | interview_score | salary
-----------|------------|-----------------|--------
           | 8          | 9               | 50000
           | 8          | 6               | 45000
five       | 6          | 7               | 60000
two        | 10         | 10              | 65000
seven      | 9          | 6               | 70000
```

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computations
  - `scikit-learn` - Machine learning (Linear Regression)
  - `matplotlib` - Data visualization (optional)

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy scikit-learn
```

### Running in Google Colab
1. Open [Google Colab](https://colab.research.google.com/)
2. Create a new notebook
3. Copy and paste the code from `simple_salary_prediction.py`
4. Run the cell (Shift + Enter)

### Running Locally
```bash
python simple_salary_prediction.py
```

## 💡 Implementation Steps

1. **Data Creation**: Create dataset from raw data
2. **Data Preprocessing**: 
   - Convert text experience values to numbers
   - Handle missing values
3. **Model Training**: Train Linear Regression model using scikit-learn
4. **Prediction**: Predict salaries for new candidates

## 📈 Results

### Model Performance
- **R² Score**: 0.9535 (95.35% accuracy)
- **RMSE**: $2,318.92

### Predictions for New Candidates

| Candidate | Experience | Test Score | Interview Score | Predicted Salary |
|-----------|------------|------------|-----------------|------------------|
| Candidate 1 | 2 years | 9 | 6 | **$51,708.98** |
| Candidate 2 | 12 years | 10 | 10 | **$93,500.84** |

### Model Equation
```
Salary = 13,538.76 + (2,952.76 × experience) + (1,849.12 × test_score) + (2,603.77 × interview_score)
```

### Feature Importance
1. **Experience**: $2,952.76 per year (Most Important)
2. **Interview Score**: $2,603.77 per point
3. **Test Score**: $1,849.12 per point

## 📁 Project Structure

```
salary-prediction/
│
├── simple_salary_prediction.py    # Main prediction script (simplified)
├── colab_complete_solution.py     # Detailed version with visualizations
├── README.md                       # Project documentation
└── requirements.txt                # Python dependencies
```

## 🔍 Key Insights

- **Experience is the strongest predictor** of salary, adding approximately $2,953 per year
- **Interview performance** is the second most important factor
- The model achieves high accuracy (95.35%) on the training data
- Each additional point in test or interview scores significantly impacts salary

## 🎓 Learning Outcomes

This project demonstrates:
- Data preprocessing and cleaning techniques
- Handling missing values and text data
- Building and training Linear Regression models
- Making predictions with trained models
- Evaluating model performance

## 🤝 Contributing

Feel free to fork this project and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.


## 👤 Author

Ojumu Oluwabukola
- GitHub: [@bouqui-x](https://github.com/bouqui-x)

- Built as a learning project for machine learning fundamentals at Tech4Dev
