# Bangla News Text Classification using Bangla-BERT

This project focuses on building a multi-class classification model for Bangla news articles. Using the **Bangla-BERT transformer model**, the system classifies text into one of several predefined categories such as Sports, National, International, Entertainment, etc.


## Dataset Description

- **Dataset Name**: `Bangla_news.csv`
- **Source**: Jamuna TV (collected for academic use)
- **Categories**: 
  - Sports
  - All-Bangladesh
  - International
  - Entertainment
  - National
- **Columns**:
  - `content`: The Bangla news article
  - `category`: The labeled category of the news


## ⚙️ Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Milon122860/Bangla_Text_Classification.git
   cd Bangla_Text_Classification


📊 Project Steps
✅ Step 1: Exploratory Data Analysis (EDA)
Checked dataset structure, class distribution, missing values.

Visualized text length distribution.

✅ Step 2: Preprocessing
Cleaned Bangla text using regex.

Removed URLs, non-Bangla characters, and stopwords.

Dropped empty rows after cleaning.

✅ Step 3: Label Encoding & Train-Test Split
Encoded category to numerical labels.

80-20 split of training and test sets using stratify.

✅ Step 4: Tokenization & Dataset Conversion
Used sagorsarker/bangla-bert-base tokenizer.

Converted to HuggingFace Dataset format and tokenized.

✅ Step 5: Model Training
Fine-tuned Bangla-BERT using HuggingFace Trainer.

Used f1 as the evaluation metric.

Trained for 1 epoch (can be tuned).

✅ Step 6: Evaluation
Evaluated with accuracy, F1, precision, recall.

Generated classification report & confusion matrix.

Calculated ROC AUC score for multi-class classification.



