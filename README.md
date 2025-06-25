
# Potential Customer Prediction

## Project Overview

This project aims to predict which leads are most likely to convert to paid customers for ExtraaLearn, an EdTech startup. By leveraging classification algorithms and hypothesis testing, the project identifies the key attributes and behaviors that drive lead conversion, enabling more efficient resource allocation and targeted marketing strategies[^1].

## Problem Statement

With rapid growth in the online education sector, ExtraaLearn faces the challenge of efficiently identifying high-potential leads from a large pool. The objective is to:

- Build machine learning models to predict lead conversion likelihood.
- Identify factors that most influence conversions.
- Provide actionable insights to optimize marketing and sales efforts[^1].


## Dataset

The dataset contains 4,612 records with the following features:

- **Demographics:** Age, current occupation (Professional, Unemployed, Student)
- **Interaction Details:** First interaction channel (Website, Mobile App), profile completion percentage, website visits, time spent on website, page views per visit, last activity (Email, Phone, Website)
- **Marketing Channels:** Exposure to newspaper, magazine, digital ads, educational channels, and referrals (all as binary flags)
- **Target Variable:** `status` (1 = converted to paid customer, 0 = not converted)[^1]

No missing values are present. Categorical variables are encoded as needed for modeling.

## Skills \& Tools Used

- **Data Analysis \& Visualization:** pandas, numpy, matplotlib, seaborn
- **Preprocessing:** Label encoding, ordinal encoding, scaling (StandardScaler)
- **Modeling:**
    - Decision Tree Classifier
    - Random Forest Classifier
    - Logistic Regression (L1/L2)
    - Support Vector Machine (SVM)
- **Model Evaluation:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix, Precision-Recall Curves
- **Hyperparameter Tuning:** GridSearchCV
- **Feature Importance Analysis**


## Key Findings

- **Top Predictors:** Time spent on website, profile completion, and first interaction channel (website) are the most influential factors for conversion.
- **Target Audience:** Older, professional leads are more likely to convert.
- **Channel Effectiveness:** Website and digital channels outperform print media and referrals, though referred leads have a higher conversion rate.
- **Model Performance:**
    - Random Forest (after hyperparameter tuning): ~84% accuracy, 79% recall for converters.
    - SVM with RBF kernel: ~84% accuracy, balanced precision/recall.
    - Logistic Regression and Decision Tree models performed slightly lower, with recall for converters in the 63–73% range[^1].


## Recommendations

- **Optimize Website Experience:** Given the strong link between website engagement and conversion, focus on improving site usability and encouraging profile completion.
- **Target Professionals:** Marketing efforts should prioritize older professionals, as they show higher conversion rates.
- **Boost Referral Programs:** Although few leads come from referrals, their conversion rate is high—expanding referral incentives could yield more paying customers.
- **Emphasize Digital Channels:** Digital marketing is more effective than print; resources should be allocated accordingly[^1].


## How to Use This Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/potential-customer-prediction.git
cd potential-customer-prediction
```


### 2. Data

Ensure you have the dataset (`ExtraaLearn.csv`) in the project directory.

### 3. Environment Setup

Install required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```


### 4. Run the Analysis

Open the Jupyter notebook or HTML file (`Potential_Customer_Prediction.html`) to review the full analysis and results.

### 5. Reproduce the Modeling

To retrain or test models:

- Load and preprocess the data as described.
- Run the provided scripts to train and evaluate models.
- Adjust hyperparameters as needed for further tuning.


## File Structure

- `Potential_Customer_Prediction.html` – Full analysis and modeling workflow[^1]
- `README.md` – Project overview and usage instructions


## Contributing

Contributions are welcome! Please open an issue or submit a pull request for improvements or additional features.

## License

This project is licensed under the MIT License.



