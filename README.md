# Word2Vec

Vector representations for words from text. The main idea is that words appearing in similar contexts have similar meanings. Because of that, word vectors of similar words should be close together. Models that use word vectors can utilize these properties, e.g., in sentiment analysis a model will learn that "good" and "great" are positive words, but will also generalize to other words that it has not seen (e.g. "amazing") because they should be close together in the vector space.
Vectors can keep other language properties as well, like analogies. The question "a is to b as c is to ...?", where the answer is d, can be answered by looking into word vector space and calculating $\mathbf{u}_b - \mathbf{u}_a + \mathbf{u}_c$, and finding the word vector that is the closest to the result.

Project for the course Machine Learning for Graphs and Sequential Data(IN2323) at Technical University of Munich. 

Implementation based on the original paper: 
* https://arxiv.org/pdf/1310.4546.pdf
