# Diabetes-dataset-Classifier-Comparison

This project compares the performance of different classification models on the Pima Indians Diabetes dataset.

## Models Compared

- Decision Tree
- Bagging Classifier
- Random Forest (with max_depth tuning)
- AdaBoost (with learning rate tuning)

## Dataset

The dataset `pima-indians-diabetes.data.csv` contains medical predictor variables and a binary target for diabetes diagnosis.

Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/pima+indians+diabetes)

##  Features

| Feature | Description |
|---------|-------------|
| preg    | Number of times pregnant |
| plas    | Plasma glucose concentration |
| pres    | Diastolic blood pressure (mm Hg) |
| skin    | Triceps skin fold thickness (mm) |
| test    | 2-Hour serum insulin (mu U/ml) |
| mass    | Body mass index (BMI) |
| pedi    | Diabetes pedigree function |
| age     | Age (years) |
| class   | 1 = diabetes, 0 = no diabetes |

## Results

The models are evaluated using:
- Single test set accuracy
- ROC curve (Random Forest)
- Cross-validation (5-fold)

### Best Models (Cross-Validation):

- **Random Forest (max_depth=5)**: Best overall accuracy
- **AdaBoost (learning_rate=0.5)**: Most balanced

## Dependencies

Install required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn
