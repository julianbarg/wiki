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

## Options
Two important options for topic modeling are [[Stemming]] and [[Lemmatizing]]. These two methods reduce words to their stems (e.g., swim instead of swimming), and thus increase the probability that a pattern is detected when a word occurs in many different forms. Stanford Core NLP can collapse two word phrases (e.g., fast food), alternatively, one can use N-grams (for example bigrams) for the analysis. Using bigrams means including in the analysis all individual terms as well as all two-word combinations of adjacent words. Stop words should be removed.

 The standard approach, as used by [[Hannigan et al. 2019]], is to maximize the likelihood of the absolute number of words by document to occur as observed in the corpus by identifying the appropriate topics. To identify the topics that maximize this likelihood, [[Latent Dirichlet Allocation]] (LDA) is used. To prevent the algorithm from being dominated by common but meaningless words such as "the", "also", or "I", a preexisting *dictionary* is used to filter out stop words such as these. The alternative approach with tf-idf entails, instead of using the absolute number of occurrences per text in the corpus, to use the absolute number divided by the share of documents containing the word. For instance, if a word is contained in all texts in the corpus, it is likely a very generic word (such as "the"). On the other hand, words that occur on in a few texts only, but very frequently in those few texts, are probably important and meaningful words. The weight of these words in the model is boosted when using tf-idf. The most and less frequent words are also often removed. The advantage of this second approach is that all steps of the process can be tuned iteratively using hyperparameters.