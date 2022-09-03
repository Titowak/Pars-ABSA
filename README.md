# Pars-ABSA
Pars-ABSA is a benchmark corpora on Persian presented in http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.763.pdf and https://arxiv.org/abs/1908.01815 for aspect-based sentimnet analysis.
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


In case of using our dataset please cite to our paper as following:


@InProceedings{shangipourataei-EtAl:2022:LREC,
  author    = {Shangipour ataei, Taha  and  Darvishi, Kamyar  and  Javdan, Soroush  and  Minaei-Bidgoli, Behrouz  and  Eetemadi, Sauleh},
  title     = {Pars-ABSA: a Manually Annotated Aspect-based Sentiment Analysis Benchmark on Farsi Product Reviews},
  booktitle      = {Proceedings of the Language Resources and Evaluation Conference},
  month          = {June},
  year           = {2022},
  address        = {Marseille, France},
  publisher      = {European Language Resources Association},
  pages     = {7056--7060},
  abstract  = {Due to the increased availability of online reviews, sentiment analysis witnessed a thriving interest from researchers. Sentiment analysis is a computational treatment of sentiment used to extract and understand the opinions of authors. While many systems were built to predict the sentiment of a document or a sentence, many others provide the necessary detail on various aspects of the entity (i.e., aspect-based sentiment analysis). Most of the available data resources were tailored to English and the other popular European languages. Although Farsi is a language with more than 110 million speakers, to the best of our knowledge, there is a lack of proper public datasets on aspect-based sentiment analysis for Farsi. This paper provides a manually annotated Farsi dataset, Pars-ABSA, annotated and verified by three native Farsi speakers. The dataset consists of 5,114 positive, 3,061 negative and 1,827 neutral data samples from 5,602 unique reviews. Moreover, as a baseline, this paper reports the performance of some aspect-based sentiment analysis methods focusing on transfer learning on Pars-ABSA.},
  url       = {https://aclanthology.org/2022.lrec-1.763}
}

