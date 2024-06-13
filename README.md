# parkinsons_disease_prediction
Parkinsons Disease Prediction Using ML

# Parkinson's Disease Prediction

This project aims to predict Parkinson's disease using machine learning techniques on a dataset containing various biomedical voice measurements.

## Dataset

The dataset consists of 195 rows and 24 columns. Each row represents a different voice measurement for a particular patient.

### Data Columns

- `name`: Name of the patient (not used in prediction)
- `MDVP:Fo(Hz)`: Average vocal fundamental frequency
- `MDVP:Fhi(Hz)`: Maximum vocal fundamental frequency
- `MDVP:Flo(Hz)`: Minimum vocal fundamental frequency
- `MDVP:Jitter(%)`: Measure of variation in fundamental frequency
- `MDVP:Jitter(Abs)`: Measure of variation in fundamental frequency
- `MDVP:RAP`: Measure of variation in fundamental frequency
- `MDVP:PPQ`: Measure of variation in fundamental frequency
- `Jitter:DDP`: Measure of variation in fundamental frequency
- `MDVP:Shimmer`: Measure of variation in amplitude
- `MDVP:Shimmer(dB)`: Measure of variation in amplitude
- `Shimmer:APQ3`: Measure of variation in amplitude
- `Shimmer:APQ5`: Measure of variation in amplitude
- `MDVP:APQ`: Measure of variation in amplitude
- `Shimmer:DDA`: Measure of variation in amplitude
- `NHR`: Measure of ratio of noise to tonal components in the voice
- `HNR`: Measure of ratio of noise to tonal components in the voice
- `status`: Health status of the subject (1 = Parkinson's, 0 = healthy)
- `RPDE`: Measure of dynamical complexity
- `DFA`: Signal fractal scaling exponent
- `spread1`: Nonlinear measure of fundamental frequency variation
- `spread2`: Nonlinear measure of fundamental frequency variation
- `D2`: Measure of signal complexity
- `PPE`: Measure of fundamental frequency variation

## Data Preprocessing

1. **Basic Info**: Obtained basic information about the dataset including null values, shape, description, and data types.
2. **Drop Unnecessary Columns**: Dropped the `name` column as it does not contribute to the prediction.
3. **Correlation and Heatmap**: Analyzed correlation between features and plotted a heatmap to visualize the relationships.

## Model Training

- **Train-Test Split**: Split the data into training and testing sets.
- **Model Selection**: Used Support Vector Classifier (SVC) as it is suitable for binary classification.
- **Evaluation Metrics**: Evaluated the model using confusion matrix and accuracy score.

### Results

- **Accuracy Score**: 0.83
- **Confusion Matrix**: 

[[ 5 10]

[ 0 44]]

## Conclusion

The SVC model achieved an accuracy of 83%, correctly predicting the majority of Parkinson's disease cases in the dataset.

## How to Run

# Clone the repository:
  ```bash
  git clone https://github.com/riitk/parkinsons_disease_prediction.git
  cd parkinsons_disease_prediction