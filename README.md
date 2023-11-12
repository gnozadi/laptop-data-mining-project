# Laptop Data Mining Project
This project analyzes laptop data to predict price ranges and identify patterns in laptop configurations.

## Project Overview
This project involves three phases: statistical comparison, frequent pattern extraction, and classification based on a laptop dataset. The dataset contains various features: price, RAM, SSD, HDD, processor brand, and rating stars.

### Phase 1: Data Cleaning and Statistical Comparison
In this phase, we perform data preprocessing and statistical comparison of each laptop’s price with the average price of laptops of the same brand. This phase involves: 

1. **Data Preprocessing**:
    - Handle missing values.
    - Identify and remove outliers from numerical data.
    - Apply data reduction techniques if necessary.
    - Convert numerical data to categorical data where needed.
    - Apply stemming, lemmatization, and remove stop words for textual data using libraries such as `nltk`.

2. **Statistical Comparison**:
    - Compare the price of each laptop with the average price of laptops from the same brand.
    - Conduct necessary statistical analysis for further insights.

### Phase 2: Frequent Pattern Extraction
In this phase, patterns are extracted between `RAM`, `SSD`, `HDD`, and the processor brand. This phase involves: 

1. **Data Preparation**: Use the cleaned dataset from Phase 1.
2. **Frequent Pattern Extraction**:
    - Identify frequent patterns between laptop components.
    - Extract meaningful insights from the data patterns.

### Phase 3: Classification of Laptop Ratings
Here, we classify the `star_rating` feature into predefined categories (low, mid, high) and perform classification. This phase involves: 

1. **Data Labeling**:
    - Categorize the `star_rating` feature:
      - `0-2`: Low
      - `2-4`: Mid
      - `4-5`: High
2. **Text Vectorization**: 
    - Convert any textual data into vectors.
3. **Classification**:
    - Implement classification with the preprocessed data to predict the `star_rating` category for test data.

---

## Libraries Used:
*   Pandas
*   NumPy
*   SciPy
*   Matplotlib
*   Seaborn
*   Mlxtend
*   Scikit-learn
  
## How to Run:
1.  Install the required libraries.
2.  Load the `laptop.csv` dataset into a Pandas DataFrame.
3.  Execute the code in the notebook to perform the analysis and generate the reports.

## Conclusion
This project successfully implemented a three-phase approach to analyze, extract patterns, and classify data from a laptop dataset. The insights from statistical comparison and frequent patterns provide valuable information for understanding price trends and hardware configurations. The classification model performed well in categorizing laptop ratings, although there is room for improvement in differentiating between `mid` and `high` ratings.

Future work could focus on fine-tuning the classification model and exploring additional features to enhance prediction accuracy.
