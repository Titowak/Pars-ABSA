# Pars-ABSA
				****Pars-ABSA Dataset****
This file demonstrates how to use Pars-ABSA corpus associated files.

Pars-ABSA consists of following files:
	Pars-ABSA_all
	Pars-ABSA_xml
	Pars-ABSA_train
	Pars-ABSA_test

Parts descriptions:
Pars-ABSA_all: there are 10,002 samples in this file that for each annotated targets from of 
Pars-ABSA_all, 3 lines are given. First line consists of comment that is related to target which 
target is replaced with $T$. At second line, target is given and at third line, related label is 
given.

Pars-ABSA_train: 8,001 samples of total 10,002 samples in Pars-ABSA_all is selected as training set 
with a similar format previously explained for Pars-ABSA_all.

Pars-ABSA_test: 2,001 samples of total 10,002 samples in Pars-ABSA_all is selected as test set with 
a similar format previously explained for Pars-ABSA_all.

Pars-ABSA_xml: there is a main tag named 'sentences' that contains all of the data samples. For 
each review in the dataset, there is a 'sentence' tag available inside the main tag. 'sentence' tag 
encompasses two types of tags, first is 'text' tag that has the review text and the second is 
'aspectTerms' that consists of one or more 'aspectTerm' tags. As long as it is possible to have 
more than one aspect in each sentence, all of the available aspects in each sentence are going to 
be inside 'aspectTerms' and for each aspect, there would be an 'aspectTerm' tag with four attributes. 
These attributes are:
	from: the starting position of aspect term in the sentence
	to: the ending position of aspect term in the sentence
	term: aspect term in the sentence
	polarity: sentiment polarity of aspect term




