# Sentiment Analysis Dataset

## Overview
This dataset is designed for **unsupervised sentiment analysis** and consists of textual reviews. Since it is **unstructured and unlabelled**, clustering techniques were used to derive sentiment labels.

## Dataset Files
- 📂 **`sentiment_dataset_1.csv`** – Original unlabelled dataset with raw text reviews.
- 📂 **`sentiment_dataset_with_labels.csv`** – Processed dataset with assigned sentiment labels.
- 📂 **`sentiment_train.csv`** – 80% of the labeled dataset used for training.
- 📂 **`sentiment_test.csv`** – 20% of the labeled dataset used for testing.

## Preprocessing Steps
### 1. Text Cleaning  
- Removed special characters, numbers, and stopwords.
- Converted text to lowercase.

### 2. Feature Extraction  
- Applied **TF-IDF Vectorization** to transform text into numerical features.

### 3. Unsupervised Clustering  
- Used **K-Means Clustering (K=5)** to group reviews into sentiment-based clusters.

### 4. Manual Label Assignment  
- Each cluster was analyzed and mapped to sentiment labels:
  - **1 - Very Bad**
  - **2 - Bad**
  - **3 - Okayish**
  - **4 - Good**
  - **5 - Very Good**

## Column Descriptions  
| Column Name | Description |
|-------------|-------------|
| `Review` | The raw text review from users. |
| `Cluster` | The assigned cluster ID from K-Means (0-4). |
| `Sentiment` | The mapped sentiment label based on manual analysis. |

## Train-Test Split
- The dataset is **split into 80% training and 20% testing**.
- 📂 **`sentiment_train.csv`** – Used to train sentiment classification models.
- 📂 **`sentiment_test.csv`** – Used to evaluate model performance.

## Usage  
- The **`sentiment_dataset_with_labels.csv`** can be used for **supervised sentiment classification**.  
- The **clustering approach** is useful for **unsupervised sentiment analysis applications**.  
- The **train-test datasets** are structured for **ML model evaluation**.

## Next Steps 🚀  
Improve clustering accuracy using **word embeddings (Word2Vec, BERT, etc.)**.  
Validate clustering with **sentiment lexicons**.  
Train a **classification model** using the labeled dataset.  

-----------------------------------------------------------------------------------------------------------------------------

