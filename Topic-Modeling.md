
Return to [[Methods]]

---

## Related to

### Other methods
* [[Latent Dirichlet Allocation]] (LDA)
* [[Natural Language Processing]] (NLP)

### Seminal papers
* [[Hannigan et al. 2019]]

### Parameters/options
* [[Lemmatizing]]
* [[N-grams]]
* [[Stemming]]
* [[Stop words]]
* [[tf-idf]]

## One-paragraph summary
Simulating the words (or N-grams) in a corpus of texts as being sampled from different topics. The researcher chooses the number of topics, and the algorithm determines the topics in a fashion that maximizes the probability to see the actual distributions of words over the individual texts in the corpus as seen in the data. For instance, the algorithm might find one group of words consistently appearing in 20% of the texts, and group those words as one topic.

## Options
[[Hannigan et al. 2019]] chose to create the topics by using the individual paragraphs in all texts as the unit of analysis. They also decide to use [[Stemming]] and [[Lemmatizing]], and Stanford CoreNLP was used by them to collapse phrases. An alternative to this approach is to use [[tf-idf]] (term frequency-inverse document frequency) in conjunction with [[N-grams]] to capture important phrases (of one or more words) while filtering out [[Stop words]]. The standard approach, as used by [[Hannigan et al. 2019]], is to maximize the likelihood of the absolute number of words by document to occur as observed in the corpus by identifying the appropriate topics. To identify the topics that maximize this likelihood, [[Latent Dirichlet Allocation]] (LDA) is used. To prevent the algorithm from being dominated by common but meaningless words such as "the", "also", or "I", a preexisting *dictionary* is used to filter out stop words such as these. The alternative approach with tf-idf entails, instead of using the absolute number of occurrences per text in the corpus, to use the absolute number divided by the share of documents containing the word. For instance, if a word is contained in all texts in the corpus, it is likely a very generic word (such as "the"). On the other hand, words that occur on in a few texts only, but very frequently in those few texts, are probably important and meaningful words. The weight of these words in the model is boosted when using tf-idf. The most and less frequent words are also often removed. The advantage of this second approach is that all steps of the process can be tuned iteratively using hyperparameters.