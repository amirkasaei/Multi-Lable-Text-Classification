# Multi-Lable-Text-Classification
Recurrent Neural Network(LSTM, GRU, etc) Multi Label Classification on Persian Sentences

## Purpose
- The purpose of this project is to learn about Data Labeling, Multi-label Classification, Text Processing and Recurrent Neural Networks.

## Description
- In this project we use [PerSICK](https://github.com/Ledengary/COPER/blob/main/Datasets/PerSICK.csv) dataset.
<div align="center"><img src="https://github.com/amirkasaei/Multi-Lable-Text-Classification/blob/main/Dataset/data.jpg?raw=true" width="90%" /></div>

  
- As you can see, this dataset contains three thousand rows and three columns. Each line contains two sentences, sentence1 and sentence2, and the degree of similarity between these two sentences is determined by score. This dataset is suitable for the task of detecting textual similarity (Textual Similarity), during which two sentences are given as input to the neural network and the degree of similarity between them is detected.
- Taking a closer look at the dataset, you will notice that the pairs of sentences are mostly about one of the topics: a child or children who do X, a cat or a dog which does Y, a man or a woman who... So it can be concluded that in general, these pairs of sentences can be classified according to the topic.
- During this project, we have to categorize these pairs of sentences based on the subject. The category of subjects that our model should be able to classify is equal to:
  - Man / Boy: (Example: A man is jumping into an empty pool. A young boy climbs a wall made of stone.)
  - Woman / girl: (Example: A woman wears an Egyptian hat. A young girl in a pink shirt is calmly lying on the grass.)
  - Child / Children: (Example: A young child is climbing a rock climbing wall inside the house)
  - Animals: (Example: The kittens are hungry. A dog is biting a can.)
  - Other: (Example: People look at some of the clothes gathered near the forest)
  - N/A: (for cases where the subject of two sentences is not the same or cannot be distinguished)
  
### This project includeds:
  1. Extracting subjects of each sentence using [Hazm](https://github.com/sobhe/hazm) library
  2. Subject Classification Neural Network to predict subject class of each sentence
  3. Preprocessing on dataset like compose score class and subject class for each sample
  4. Multi Label Classification RNN to predict score and subject class
    
Neural Networks models implemented by Keras in Tensorflow library.

## Team members
    
- Amir Kasaei    
- Amir Ezzati   
    
**This project was a pair work that we did as fourth project of Deep Learning course at University of Guilan in Jun 2022.**
