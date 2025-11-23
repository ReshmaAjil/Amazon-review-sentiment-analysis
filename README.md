
Amazon Reviews – Sentiment Analysis (In Progress)
📝 Project Overview
This project focuses on performing sentiment analysis on Amazon Book Reviews using Natural Language Processing (NLP) techniques.
Currently, progress includes:
Loading dataset
Merging reviews and product metadata
Creating sentiment labels
Extracting a sample for faster processing
Cleaning review text (lowercasing, removing stopwords, lemmatization)
Displaying first few cleaned results
Model training and TF-IDF vectorization will be added in the next phase.

🗂 Dataset
Downloaded from Kaggle: Amazon Books Reviews dataset
Contains 3 million review rows with review details and metadata.

Applied Cleaning to Sample (200,000 rows)


sample = merged.sample(200000, random_state=42)
sample["cleaned_text"] = sample["review/text"].astype(str).apply(clean_text)
sample.head()

📍 Current Status
✔ Data loaded
✔ Reviews merged
✔ Sentiment labels created
✔ Sample selected
✔ Text cleaned
✔ Ready for vectorization and model training

⏭️ Next Steps
TF-IDF vectorization
Train a classifier (Logistic Regression / Naive Bayes)
Evaluate model accuracy
Visualize sentiment distribution
Deploy results / Upload final model
