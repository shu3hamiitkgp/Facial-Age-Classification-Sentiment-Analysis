# DSAEM-FinalProject
Final project for course Data science and eng methods taken in Fall'22. The project involves two parts - 

1) Facial Age Classification
2) Sentiment Analysis on Amazon Reviews

## Facial Age Classification

Our study is focused on developing a deep learning model to classify facial images into a range of age bands, the data used is taken from Kaggle - face age detection dataset (https://www.kaggle.com/datasets/arashnic/faces-age-detection-dataset)

We develop two models - 

1) 2 layer CNN
2) Pre-trained ResNet50 Architecture

The dataset has a variety of facial images (~20K) of different individuals labeled in three age ranges - Young, Middle and Old. 

## Pre-processing and Modeling

- The data required basic preprocessing like resizing, scaling and structuring into arrays to qualify for training
- We dropped the sizes of images to 150 and 100 respectively, as the process was computationally extensive
- We used stratified splitting to overcome class imbalance to a certain extent

## Results and Model Comparisons

- With CNN model we were able to achieve a significantly higher accuracy (~87%)on the data with a difference of ~30%.
- One major factor that we observed in down-performance of Resnet50 was the class imbalance due to which the correct predictions for classes like ‘Old’ and ‘Young’ were minimal.

--------------------------------------------------------------------------------------------------------------------

## Sentiment Analysis : Data Scraping & Naive Bayes Application

- For the Naive Bayes Classifier we have used the review’s data of Apple Airpods (2nd Gen.) from Amazon.
- For HTML document’s parsing , beautifulsoup package is used along with requests_html library to make parsing simple and intuitive.
- There was high imbalance in the reviews with 87% positive response and 13% negative response.
- Bag of words CountVectorizer is used to convert the words present in the corpus into vector form , on the basis of the frequency (count) of each word that occur in the entire text.
- In this analysis we used Multinomial  Naive Bayes Algorithm. The classifier algorithm guesses the tag of a text using Bayes theorem and calculates each tag’s likelihood for the given sample and outputs the tag with the greatest chance.
- The accuracy of the model turned out to be 96.6%

Please have a look at the deck attached for a more detailed report. 
