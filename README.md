# Tweet-classification
Try to compare the performance of different model


The data, you could download from the following site:
http://thinknook.com/wp-content/uploads/2012/09/Sentiment-Analysis-Dataset.zip

This is basic NLP problem, using the keras to run the problem by using CNN, LSTM and RNN. Compare the difference of those layers.  

So what I do is quite simple, first create dictionary of word and their couting. I drop those words that appear more than 10000. Then try to represente the sentence by the index in the dictionary. If the word is outside of the dictionary, I will represente those words by 1. Then using the padding function, so each sentence could have the same size.  

The first layer of this network is Embedding layer to get high dimension feature of sentence, then using LSTM, simpleRNN or CNN.  For the loss function is the binary_crossentropy, for the gradient I use the adam, using the accuracy to be the metrics    
#### Actually, this one is quite simple, try to use the word2vec or glove to improve the performance.
