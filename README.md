# NLP Language Classifier Assignment:

Given the assignment of coding a language classifier able to distinguish between english and non-english texts I decided
 to choose the genesis corpus wich contains the entirety of the first book of the old testament in various languages.
I decided to select one of the two possible english versions of the text, in particular the King James Version, and two
 of the non-english versions, the finnish and portuguese ones.
in the end I obtained a pretty big corpus size.
For the training and testing sets I decided to use a 75%-25% ratio and made sure to shuffle the sentences so that both 
the sets contained a part of each language.
```
The performances resulted in
	Accuracy of 	0.993263
	Precision of 	1.000000
	Recall of 	0.989446
	F1 of 		0.994695
```
this kind of values make me think that maybe the languages chosen english, finnish and portuguese are almost completly
different in terms of words so the classifier has an easy work. Maybe choosing more germanic languages will make the 
classifier less precise and accurate given the possible similarities.

We could employ this classifier as a Language Probabilistic Model given that it determines the probability of each sen-
tence being written in a certain language by computing the probability of each word.
After doing so for each language given it selets the highest probability and than labels the sentence as english or not english.

link to the code(Classifier.ipynb):
