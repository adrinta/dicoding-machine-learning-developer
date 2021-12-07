# Classifying News Topic
 
The dataset contains the headline news and the topics/categories of the news. This task asks to classify news categories based on the headlines of the news.

## Data

**Data Source** = http://mlg.ucd.ie/datasets/bbc.html

![alt_text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Natural%20Language%20Processing/Assets/Data.png)

Attribute Information:

1. headlines : News Headlines
2. category : News Topics

## Data Preprocessing

**Text Cleaning** :
- Replace newlines with whitespace
- Remove redundant/multiple whitespace
- Change the text into lowercase
- Remove stopwords
- Do lemmatization

**One Hot Encoding** :

![alt_text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Natural%20Language%20Processing/Assets/OHE.png)

## Model Architecture

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Natural%20Language%20Processing/Assets/Model%20Architecture.png)

## Results

**Learning Graph**

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Natural%20Language%20Processing/Assets/Learning%20Graph.png)

**Result (Accuracy. F1 Score, Recall, Precision)**

![alt_text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Natural%20Language%20Processing/Assets/Result.png)
