Return to [[Methods]]

---

## Related to

### Other methods
* [[Latent Dirichlet Allocation]] (LDA)
* [[Natural Language Processing]] (NLP)

### Seminal papers
* [[Blei, Ng and Jordan 2003]] (method)
* [[Hannigan et al. 2019]] (application in business business science)
* [[Phan, Nguyen and Horiguchi 2008]] (Gibbs Sampling)

### Links/tools
* [[http://mallet.cs.umass.edu/import.php]]

### Parameters/options
* [[Lemmatizing]]
* [[N-grams]]
* [[Stemming]]
* [[Stop words]]
* [[tf-idf]]

## One-paragraph summary
Simulating the words (or N-grams) in a corpus of texts as being sampled from different topics. The researcher chooses the number of topics. The algorithm then identifies topics (consisting of words and weights) that maximize the probability to see the distributions of words over the individual texts in the corpus as seen in the data. For instance, the algorithm might find one group of words consistently co-occuring in 20% of the texts, and group those words as one topic.

The standard approach, as used by [[Hannigan et al. 2019]], is to maximize the likelihood of the absolute number of words by document to occur as observed in the corpus by identifying the appropriate topics. To identify the topics that maximize this likelihood, [[Latent Dirichlet Allocation]] (LDA) is used. To prevent the algorithm from being dominated by common but meaningless words such as "the", "also", or "I", a preexisting *dictionary* is used to filter out stop words such as these. The alternative approach with tf-idf entails, instead of using the absolute number of occurrences per text in the corpus, to use the absolute number divided by the share of documents containing the word. For instance, if a word is contained in all texts in the corpus, it is likely a very generic word (such as "the"). On the other hand, words that occur on in a few texts only, but very frequently in those few texts, are probably important and meaningful words. The weight of these words in the model is boosted when using tf-idf. The most and less frequent words are also often removed. The advantage of this second approach is that all steps of the process can be tuned iteratively using hyperparameters.

## Description
Topic modeling is a machine learning technique from the area of natural language processing (NLP), for work with text data. Topic modeling allows for the *unsupervised learning* of topics that occur within a corpus (collection) of texts; unsupervised because an algorithm determines which words fall into which topics, with no further guidelines on the topics provided as input from the user except for the texts themselves. The most common form of topic modeling, described in the following (henceforth called topic modeling), uses Latent Dirichlet Allocation (LDA) and was first introduced by [[Blei, Ng and Jordan (2003)|Blei, Ng and Jordan 2003]]. 

Topic modeling follows a bag-of-words approach: the order of words within text in the corpus is disregarded, and only their frequency within each text is used for the analysis. As the input, the user provides an m by n term-document matrix, where m is the number of documents, and n is the number of individual words or N-grams; N-grams being combinations of 1 through n consecutive words in the text. For instance, bigrams describes a set of terms that includes all individual words from the corpus as well as all combinations of two words that occur in the text together as neighbors (e.g., "together", "together as", "as", "as neighbors", "neighbors", etc., in this sentence). The LDA algorithm takes as input the n by m term-document matrix and returns as output an n by k matrix of weights, where k is the selected number of topics. The value a<sub>n,k</sub> for instance describes the weight of the nth word for the kth topic. k is the most important parameter to tune, because only with a sufficient number of topics will these topics become separated enough to be interpretable. 

Typically, words have high weights for one topic and low weights for all other topics, but words can have elevated weights for multiple topics as well. By extracting the words with the highest weights for each topic, the user can determine the meaning of this topic. For example, if the words with the highest weights are "business", "revenue", and "manager", it would not be too far fetched to classify this as a business topic. To determine what topic a text falls into, one takes a vector with all the words that occur in the text (and their frequency) and multiplies these with the weights for the target topic. If we take for instance the sentence "How do you do", and the weights for topic a are .10 (how), .03 (do), and .50 (you), the overall weight for that topic would be .66. By comparing the weight 




The output of the algorithm is an N by M matrix, where N is the number of individual terms provided as input
Topic modeling works with the bag of words

### Options
Two important options for topic modeling are [[Stemming]] and [[Lemmatizing]]. These two methods reduce words to their stems (e.g., swim instead of swimming), and thus increase the probability that a pattern is detected when a word occurs in many different forms. Stanford Core NLP can collapse two word phrases (e.g., fast food), alternatively, one can use N-grams (for example bigrams) for the analysis. Using bigrams means including in the analysis all individual terms as well as all two-word combinations of adjacent words. Stop words should be removed.

