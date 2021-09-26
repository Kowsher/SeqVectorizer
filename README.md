# SeqVectorizer
The latest strategies for learning vector space portrayals of words have prevailed with regards to catching fine-grained semantic and syntactic consistencies utilizing vector arithmetic, however, the sequence representation is not present to these methods. As a result, to consider the sequence we are utilizing the sequence neural networks like RNN or statistical techniques like HMM. To represent the sequence through every state vector, we propose a new term or word representation technique called SeqVectorizer which stands for sequence vectorizer. In SeqVectorizer every state represent a combined vector of two separate joined state and these are the previous sequence state and the current state probability. Comparing with other representation systems, it shows a state of the art performance on some testing data-sets.
In order to represent the previous state information through a sequence representing, we have developed heuristic model architecture name sequence vectorizer that represents previous sequence in on every current state. This decision has a few valid justifications - effortlessness, strength, and most viable is sequence representation so that common machine learning algorithms can handle the problems of sequence. 
In the procedures, every sate discloses as a probability then marge the state with the previous state using some mathematical operation. This means every current state presents two representations in a single vector the current probability of its own and the previous representation. Thus the last state can be considered as the representation of while text. In the beginning, a frequency or lookup table has to develop where every state exposes its probability as a term frequency. Then it associated in state vector representation like Markov of chain model. 
In addition, we have developed a python module name SeqVectorizer to use this term representation system and it is suitable to use any kind of machine learning algorithm. We also examined and solved some NLP problems and compared with other  existing techniques like Tf-Idf, word2vec etc where the SeqVectorizer proved a standard representation.

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


