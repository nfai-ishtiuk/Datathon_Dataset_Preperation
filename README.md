# Datathon Dataset Preparation

This project is dedicated to preparing a dataset for an upcoming datathon competition. The process includes data sourcing, preprocessing, feature engineering, and generating stratified training and testing splits for fair and balanced distribution.

## Folder Structure

The project has the following folder structure:

```
D:\NeuralFrameAi_Office\PROJECTS\Datathon_Dataset_Preperation
│
├── README.md                             # Project overview and instructions
├── dataset_preperation.ipynb             # Main notebook for dataset preparation
├── Datathon_Dataset_Sourcing_Report.pdf  # Report documenting data sourcing and cleaning
│
├── output_datasets                       # Folder containing the final prepared train and test datasets
│   ├── Air_Quality_Train.csv             # Training dataset after preprocessing and splitting
│   └── Air_Quality_Test.csv              # Testing dataset after preprocessing and splitting
│
└── selected_datasets                     # Folder containing the raw source dataset before processing
    └── Air_Quality.csv                   # Original selected dataset
```

## Project Overview

### Objectives

1. **Data Sourcing:** Obtain a high-quality dataset of over 18,000 rows from reliable sources. For this project, we focused on air quality data.
2. **Data Cleaning and Preprocessing:** Handle missing values, encode categorical features, scale numerical features, and engineer date-related features as needed.
3. **Dimensionality Reduction:** Use PCA for feature reduction to improve model interpretability and performance.
4. **Dataset Splitting:** Apply a stratified train-test split to ensure class balance across splits.

### Notebook Description

- **`dataset_preperation.ipynb`**: This notebook contains the complete pipeline, from loading the raw data to splitting and saving the processed dataset. Key sections include:
  - Data loading and initial exploration
  - Feature engineering, including PCA and date handling
  - Regression model evaluations to assess feature importance
  - Stratified train-test splitting for balanced classes in each split

### Output Files

The `output_datasets` directory contains the final processed datasets:
- **`Air_Quality_Train.csv`**: Processed training data with balanced distributions.
- **`Air_Quality_Test.csv`**: Processed testing data, ready for model evaluation.

These files are in CSV format, ready for participants to use in their machine learning workflows.

## Project Reports

- **`Datathon_Dataset_Sourcing_Report.pdf`**: Detailed documentation covering data sourcing, selected data sources, and the rationale for data selection. This report ensures transparency for datathon sponsors.

## Requirements

The project requires Python, with the following key libraries:
- `pandas` for data manipulation
- `sklearn` for model training and preprocessing
- `numpy` for numerical operations
- `plotly` and `seaborn` for data visualization

## Usage

1. Clone this repository to your local machine.
2. Run the `dataset_preperation.ipynb` notebook to recreate the dataset preparation steps.
3. Review the final train and test datasets in the `output_datasets` folder.

```bash
# Clone the repository
git clone https://github.com/yourusername/Datathon_Dataset_Preperation.git
```

### Running the Notebook

To execute the notebook:
1. Ensure all required Python libraries are installed.
2. Open and run `dataset_preperation.ipynb` in a Jupyter environment.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

Created by [Md. Ishtiuk Ahammed](https://github.com/nfai-ishtiuk), AI Engineer at NeuralFrame AI.