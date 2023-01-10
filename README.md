# Cyber-Bully-twitter-tweet-Classiifcation
Tweet classification using NLP

🧾Description: This dataset is a collection of datasets from different sources related to the automatic detection of cyber-bullying. The data is from different social media platforms like Kaggle, Twitter, Wikipedia Talk pages, and YouTube. The data contains text and are labeled as bullying or not. The data contains different types of cyber-bullying like hate speech, aggression, insults, and toxicity. We have been provided with the twitter_parsed tweets dataset, wherein we have to classify whether the tweet is toxic or not.

The target variable is oh-label and the evaluation metric is F1-score.

Source of dataset & data dictionary - https://www.kaggle.com/datasets/saurabhshahane/cyberbullying-dataset


## 🧾 Description: 
This dataset is a collection of datasets from different sources related to the automatic detection of cyber-bullying. The data is from different social media platforms like Kaggle, Twitter, Wikipedia Talk pages, and YouTube. The data contains text and are labeled as bullying or not. The data contains different types of cyber-bullying like hate speech, aggression, insults, and toxicity.

### :bar_chart: Exploratory Data Analysis:
* Exploratory Data Analysis is the first step of understanding your data and acquiring domain knowledge. 

### :hourglass: Data Preprocessing:
* The given data was cleaned & preprocessed by first removing the unwanted special characters and numbers from text.
* Next I removed the stop words from the sentences.
* Now I used **WordNetLemmatizer** for converting each of the tokens to their root words.
* Once the data is cleaned, I used **WordEmbedding** technique to convert words into vectors.

### ☁️ Word Cloud
![Toxic Word Cloud](https://github.com/Abhissaro/Cyber-Bully-twitter-tweet-Classification/blob/288a0256452709dd129e138ad4963711e3595adb/world%20cloud.png)

### ⚙ Model Training:
* The model is trained using **BidirectionalLSTM** with a vocabulary size of 16K and each word reprented by a vector of length 300.
* My trained model gives an accuracy of **94.76%** on train data while of **81%** on test data.
* As per the problem statement I used **F1 Score** as the evaluation metric for my model.
