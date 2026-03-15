Movie Genre Classification
Welcome to my movie genre classification project! I built this supervised learning pipeline to automatically classify movie genres based purely on their textual plot summaries.

The Problem
Categorizing movies by genre just by reading a short description is a classic Natural Language Processing (NLP) challenge. In real-world datasets, text is often messy, and certain genres dominate the data while others appear very rarely. This severe class imbalance makes it difficult for machine learning models to accurately identify the minority classes.

What I Did in the Code
Here is a brief overview of my approach and the steps I took to solve this problem:

Text Processing (NLP): I started by thoroughly cleaning the data. Then, I used TF-IDF vectorization to convert the textual plot summaries into a numerical format that my models could understand, extracting the top 5,000 features to capture the most relevant vocabulary.
Tackling Class Imbalance: To address the severe disparity between genre frequencies, I engineered a solution using Oversampling techniques. This was a critical step that allowed the models to learn from minority classes effectively.
Model Training & Comparison: I implemented, trained, and compared two different models to evaluate their performance: a Linear SVC (Support Vector Classifier) and a Multi-Layer Perceptron (Neural Network).
Visualization: To get a clearer picture of how my models were separating the different genres, I applied t-SNE to visualize the high-dimensional decision boundaries.
Results
By effectively handling the class imbalance and refining the NLP pipeline, I successfully improved the model's F1-Score from a baseline of 45% to 89.28%.

Tech Stack
Python
Scikit-Learn
Pandas
NLP (TF-IDF)
