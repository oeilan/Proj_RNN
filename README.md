IMDB positive / negative sentiment classification RNN
Two models of 3 layers were implemented to predict sentiment of movie reviews: (!) Embedding - LSTM - Dense (2) Embedding - Bidirectional LSTM - Dense
Both models have around 200k of trainable parameters, took about 560+ seconds per epoch to train, and attained lowest loss and highest test accuracy of around 87% within a few epochs. Model 2, the bidirectional model, however, was able to attain 87% accuracy earlier (at 3rd epoch) compared to the first (at 7th epoch)
Dataset: 25,000 train and 25,000 test movie reviews were downloaded from keras.datasets. Reviews are of variable length of 7 to 2494 words. Words are represented by single integer index. There is a total of 5,967,841 words in all reviews, drawn from a vocabulary of 88,587
