# Speaker Age Prediction Using Linear Regression

This project aims to predict the age of speakers based on audio features extracted from a large dataset using a linear regression model. The workflow involves data extraction, preprocessing, visualization, normalization, and model comparison. 

# Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Workflow](#workflow)
  - [Feature Extraction](#feature-extraction)
  - [Data Formatting](#data-formatting)
  - [Data Preprocessing](#data-preprocessing)
    - [Handling Missing Values](#handling-missing-values)
  - [Data Visualization](#data-visualization)
  - [Normalization](#normalization)
  - [Model Development](#model-development)
  - [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributions](#contributions)
- [License](#license)

## Project Overview

The project involves predicting the age of speakers from audio files by applying a linear regression model. The approach includes custom implementations of linear regression and various preprocessing techniques, followed by comparisons with scikit-learn's built-in models.

### Dataset

- **Training Data**: Approximately 15,000 audio files.
- **Testing Data**: Approximately 4,000 audio files.

### Workflow

1. **Feature Extraction**: Features were extracted from the audio files to be used for training and testing the models.
2. **Data Formatting**: The extracted features were formatted into `training_data_features.xlsx` and `testing_data_features.xlsx`.
3. **Data Preprocessing**: Various preprocessing steps were applied to clean and prepare the data for modeling.
   - **Handling Missing Values**: Three techniques were used:
     - Dropping NaN values.
     - Filling NaN values with the mode of the feature.
     - Predicting NaN values using a separate model and then using these predictions for age prediction.
4. **Data Visualization**: 
   - Initial visualization was performed using `matplotlib` to explore relationships between different features.
   - Post-normalization visualization to assess the effect of normalization on feature relationships.
5. **Normalization**: The data was normalized to ensure consistent scaling of features.
6. **Model Development**:
   - Developed a linear regression model from scratch.
   - Implemented and compared this custom model with scikit-learn's linear regression model.
7. **Model Evaluation**:
   - Calculated Mean Squared Errors (MSE) for model performance evaluation.
   - Compared results of the custom linear regression model and the scikit-learn model across different preprocessing techniques.

### Results

The project compares the performance of different preprocessing methods and models, assessing their effectiveness in predicting speaker age. The results include performance metrics and visualizations to demonstrate the impact of various techniques on model accuracy.

### Installation

To run this project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/ZainUlWahab/speaker-age-prediction.git
   cd speaker-age-prediction

3. MAKE SURE TO UNZIP THE 'dataset.zip' if you want to extract the features again. I have attached the extracted features in 3 seperate files called 'testing_data_features.xlsx', 'training_data_features.xlsx' and 'truncated.csv'.
    
4. Run the Jupyter notebook:
   ```bash
   jupyter notebook

5. Open the speaker-age-prediction.ipynb notebook and run the cells.
   
7. If you don't want to extract the features again make sure to run the cells only after the heading "Run from here pls"
   
### Usage

To use this project, follow the steps outlined in the provided code to load the data, preprocess it, train the models, and evaluate their performance. Everything is explained in the jupyter notebook.

### Contributions

Contributions to this project are welcome! If you have suggestions for improvements or encounter any issues, please submit a pull request, open an issue on GitHub or you can contact me on my email 'ulwahabzain@gmail.com'.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
