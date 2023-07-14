# **Text Classification Analysis**

## **Introduction**

In this notebook I analyzed the dataset present with the following link: https://www.kaggle.com/datasets/vyhuholl/japanese-newspapers-20052021 (in the English version) of which discusses Japanese newspaper articles from two editorial: Mainichi Shimbun and The Japan Times.

The goal is to analyze the dataset which is highly unbalanced, find common repeating patterns, and perform a binary classification.

The dataset having textual features was chosen to use NLP (Natural Language Processing) and Word Embedding techniques in order to have a numerical representation and interpretable by the algorithms.

Finally, exploit these features to be able to predict, given the text of a paper, which editorial staff it was written by.

---

## **Design Choices**

In this section, the adopted project pipeline will be analyzed.

1. **Language and Development Environment:** Python was chosen as the programming language, and Jupyter Notebook was selected as the development environment. This combination provides a wide range of libraries and facilitates exploratory data analysis. Google Drive was chosen to store and upload all data.

2. **Data Manipulation:** The dataset "english_news.csv" was loaded, and missing values (NaN) in the "author" field were handled. Records with NaN in the "author" field were retained as they account for approximately 35% of the data and are relevant for analysis.

3. **Author Analysis:** An analysis of the authors in the dataset was conducted, including visualizations to examine the author distribution. It was observed that many authors appeared only once, while a minority of authors had multiple occurrences.

4. **Class Imbalance:** Various techniques were explored to address class imbalance in the dataset, including oversampling, undersampling and smoothing. The impact of records with NaN on class balance was evaluated.

5. **Pre-processing:** As a result of the previous analyses, the dataset was manipulated according to various strategies, leveraging NLP and Word Embedding with pre-trained models. 
All these configurations were saved within Google Drive.

6. **Machine Learning Approach:** Initially it was decided to use machine learning algorithms such as SVC and Random Forest to perform binary classification trying to avoid overfitting by weighting the classes differently.These algorithms were evaluated with various metrics such as Precision, Recall, F1, Accuracy and AUC curves.

7. **Deep learning approach:** Deep learning techniques were incorporated into the analysis. Preprocessing of textual data was performed using techniques such as tokenization and embedding. Neural network architectures, including convolutional neural networks (CNNs), were implemented for classification tasks.


This adopted pipeline was made to effectively manage the data, address class imbalance, and leverage deep learning and machine learning techniques to gain meaningful insights in text analysis.