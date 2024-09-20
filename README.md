

# MBA Admission Analysis

This project aims to predict MBA admissions decisions (Admit, Waitlist, Deny) using machine learning models based on candidate information such as gender, international status, GPA, major, race, work experience, work industry, and GMAT scores.

## Project Overview

In this project, I perform exploratory data analysis (EDA), preprocess the data, and build two machine learning models:
- **Linear Regression** for predicting admission outcomes.
- **Decision Tree Classifier** for classifying admissions decisions.

### Features Used:
- **Gender**
- **International Status**
- **GPA**
- **Major**
- **Race**
- **Work Experience**
- **Work Industry**
- **GMAT Score**

### Repository: 
[devkverma/MBA-admission-analysis](https://github.com/devkverma/MBA-admission-analysis)

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/devkverma/MBA-admission-analysis.git
   cd MBA-admission-analysis
   ```

2. **Create and activate a virtual environment (optional)**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset

The dataset used contains anonymized information about MBA applicants and their admissions status. It includes the following columns:
- `gender`
- `international`
- `gpa`
- `major`
- `race`
- `work_exp`
- `work_industry`
- `gmat`
- `admission` (target variable)

## Data Preprocessing

- Handled missing data by filling categorical columns with the mode.
- Encoded categorical columns using `LabelEncoder` for the machine learning models.
- Split the data into training and test sets using an 80-20 ratio.

## Models

### 1. **Linear Regression**
   - Trained a linear regression model to predict admission outcomes.
   - **Evaluation**: Mean Squared Error (MSE).

### 2. **Decision Tree Classifier**
   - Built a decision tree classifier for admissions classification.
   - **Evaluation**: Accuracy score.

## Visualization

- Pie charts for analyzing the distribution of categorical features (gender, race, major, international status, work experience, work industry).
- Bar plots showing average GMAT scores by gender and major.

## Results

- **Linear Regression** model evaluated using Mean Squared Error (MSE).
- **Decision Tree Classifier** achieved a satisfactory accuracy score for predicting MBA admissions decisions.

## Usage

To test the model with new data:

```python
data = pd.DataFrame({
    'gender': [1],
    'international': [1],
    'gpa': [3],
    'major': [1],
    'race': [4],
    'work_exp': [1],
    'work_industry': [1],
    'gmat': [600]
})

prediction = model_decision_classifier.predict(data)
print(prediction)
```

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Contributing

Feel free to submit issues or pull requests.

## Contact

For any inquiries, please reach out to me at devverma269@gmail.com.

