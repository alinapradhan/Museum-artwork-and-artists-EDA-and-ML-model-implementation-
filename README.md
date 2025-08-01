
# MoMA Art Analysis & Classification

This project performs exploratory data analysis on the Museum of Modern Art (MoMA) collection and builds a machine learning model to classify artworks based on metadata like Nationality, Department, and Medium.

##  Features

- Cleans and merges data from Excel sheets 
- Visualizes gender distribution, acquisition trends, continents of origin, and mediums
- Builds a Random Forest Classifier to predict artwork classification

## Dataset

- Source: `MoMA_OnView.xlsx`
- Sheets used: `Artworks`, `Artists`

## ML Model

- **Type**: Random Forest Classifier
- **Target**: `Classification`
- **Features**: `Nationality`, `Department`, `Medium`
- **Preprocessing**: Label encoding, missing value imputation

## How to Run

1. Install dependencies:
    ```bash
    pip install pandas scikit-learn matplotlib seaborn openpyxl
    ```

2. Place `MoMA_OnView.xlsx` in the same directory.

3. Open and run the notebook:
    ```bash
    jupyter notebook PROJECT.ipynb
    ```

## Visualizations

- Gender distribution of artists
- Top 10 contributing artists
- Artwork origin by continent (pie & donut charts)
- Acquisition trend over time
- Medium popularity

## Example ML Prediction

```python
predict_classification("American", "Painting", "Oil on canvas")
