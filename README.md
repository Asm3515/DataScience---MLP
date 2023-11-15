# DataScience---MLP
# Word2Vec Pretrained Models Report

## Author: Ajinkya Shekhar More
### Assignment Date: 13th November 2023

### Introduction:
This report explores the application of Word2Vec and its pretrained models to train a Language Model (LM) in Python. It evaluates model performance, compares algorithm accuracy before and after improvements, and analyzes the impact of data preprocessing.

### SPLIT_DATA Function:
The `split_data` function is implemented in Python 3.9 within the PyCharm environment. It reads, preprocesses, tokenizes, and splits a CSV file, playing a crucial role in the project. Key steps include CSV opening, data preprocessing (sentiment transformation), data splitting, and saving split data in CSV format.

### SAVE_TRAIN_TEST_FILES Function:
This function opens a CSV file, preprocesses data, splits it into training and testing sets, and saves the split data into separate CSV files based on specified percentages.

### load_imdb_dataset Function:
This function opens a CSV file containing the IMDB dataset, extracts features (reviews) and targets (sentiments), prepares data for training, and returns extracted features and targets for further analysis.

### train_MLP_model_average Function:
This function converts text data into average word embeddings using a pretrained Word2Vec model, transforms text data into numerical representations, trains a Multi-Layer Perceptron (MLP) model, and returns the trained model for testing.

### train_MLP_model_student Function:
This function creates word embeddings using a specific logarithmic transformation from Word2Vec models, handles missing embeddings to avoid errors, trains an MLP model using modified word embeddings, and returns the trained model with student-specific embeddings.

### test_MLP_model Function:
This function reads a test dataset, prepares features (numerical representations), predicts sentiments using a trained model, evaluates accuracy, and saves the output to a CSV file.

### Output Results:

- **Average Embedding Model Accuracy**: 81.4%
- **Student Embedding Model Accuracy**: 81.22%

### Output Observations:

1. **Baseline Accuracy:** Pretrained Word2Vec models show strong baseline accuracy, exceeding 81%, indicating effectiveness in sentiment analysis.

2. **Confusion Matrix Analysis:** Balanced matrices for both models highlight accurate predictions, demonstrating Word2Vec embeddings' robustness in handling diverse sentiment patterns.

3. **Comparison with Logistic Regression:** Word2Vec models, even with basic preprocessing, rival logistic regression, achieving accuracy over 70%, showcasing natural language understanding prowess.

4. **Impact of Preprocessing:** Effective preprocessing, including sentiment transformation and data splitting, significantly contributes to high model accuracy.

5. **Embedding Generation Impact:** The use of average and student-specific embeddings showcases Word2Vec's adaptability, providing diverse embeddings for improved sentiment analysis outcomes.

6. **Handling Missing Embeddings:** The Student Embedding Model's resilience to missing words, managed through logarithmic transformations, ensures a robust training process with minimized errors.

This report underscores the efficacy of Word2Vec pretrained models, emphasizing their adaptability, competitive accuracy, and potential across various natural language processing tasks.
