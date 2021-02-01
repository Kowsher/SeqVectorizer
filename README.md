# SeqVectorizer
The latest strategies for learning vector space portrayals of words have prevailed with regards to catching fine-grained semantic and syntactic consistencies utilizing vector arithmetic, however, the sequence representation is not present to these methods. As a result, to consider the sequence we are utilizing the sequence neural networks like RNN or statistical techniques like HMM. To represent the sequence through every state vector, we propose a new term or word representation technique called SeqVectorizer which stands for sequence vectorizer. In SeqVectorizer every state represent a combined vector of two separate joined state and these are the previous sequence state and the current state probability. Comparing with other representation systems, it shows a state of the art performance on some testing data-sets.

![Alt text](https://github.com/Kowsher/SeqVectorizer/blob/main/seq.png?raw=true "Title")

To install just follow the command

```python
pip install SeqVectorizer
```

This is a simple API just to use, Very soon, we are going to develop a high module on tensorflow 
To use just follow


```python
from SeqVectorizer import Vectorizer
vec = Vectorizer()
x_train = vec.fit_transform(train_sentences)
x_test = vec.transform(test_sentences)
```

to get the all term's set

```python
vec.get_features()
#to get the vocabulary
```

In our experiment, we incorporated three popular datasets, i.e., Amazone Food Review4, Amazon Product Review5 and IMBD Movie and compared with existing popular algorithms like wor2vec, fasstext, glove, tf-idf

![Alt text](https://github.com/Kowsher/SeqVectorizer/blob/main/amazon.png?raw=true "Title")

![Alt text](https://github.com/Kowsher/SeqVectorizer/blob/main/amazon6.png?raw=true "Title")

![Alt text](https://github.com/Kowsher/SeqVectorizer/blob/main/imdb.png?raw=true "Title")


