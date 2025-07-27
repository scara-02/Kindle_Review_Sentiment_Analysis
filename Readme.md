# 📚 Kindle Review Sentiment Analysis

A Natural Language Processing (NLP) project that classifies Amazon Kindle product reviews as **positive** or **negative** using text preprocessing and a Logistic Regression classifier. This model achieved an accuracy of **82%** on the test dataset.

---

## 🚀 Project Objective

To build a sentiment classification system that helps determine whether a given Kindle review expresses a **positive** or **negative** sentiment. This helps potential buyers quickly understand the overall perception of the product.

---

## 🧠 Project Workflow

### 1. 📥 Dataset
- **Source**: `all_kindle_review.csv` (This dataset is taken from Amazon product data, Julian McAuley, UCSD website. http://jmcauley.ucsd.edu/data/amazon/).
- **Size**: 12000 reviews.
- **Format**: Each row contains a text review and its ratings[1-5].

### 2. 🧹 Data Preprocessing
- Removed HTML tags, special characters, numbers, and punctuations.
- Converted text to lowercase.
- Removed stopwords using `nltk`.
- Tokenized and lemmatized the reviews.
  
### 3. 🔢 Feature Engineering
- **Word2Vec Vectorization** was applied to convert text into numerical features.
- Limited vocabulary to top N features to reduce dimensionality and overfitting.

### 4. 🧪 Model Building
- **Algorithm Used**: Logistic Regression (`sklearn.linear_model`)
- **Train-Test Split**: 80% training and 20% testing.
- **Hyperparameters**: Default settings with minor tuning.

### 5. 📊 Model Evaluation
- **Accuracy**: `85%`
- **Precision**: 0 : 82%   ,  1 : 82% calculated
- **Recall**: 0 : 82%   ,  1 : 82% calculated
- **F1-Score**: 0 : 82%   ,  1 : 82%  calculated.


## 📈 Results

| Metric       | Score |
|--------------|-------|
| Accuracy     | 82%   |
| Precision    | 82%   |
| Recall       | 82%   |
| F1-Score     | 82%   |



## 🧰 Tech Stack

| Area                 | Tools & Libraries                           |
|----------------------|---------------------------------------------|
| Programming Language | Python                                      |
| Text Processing      | NLTK, re, string                            |
| Feature Extraction   | Scikit-learn (TF-IDF)                       |
| Model                | Logistic Regression (Scikit-learn)          |
| Visualization        | Matplotlib, Seaborn                         |
| Development          | Jupyter Notebook, VS Code                   |

---

