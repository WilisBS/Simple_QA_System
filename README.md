# Simple_QA_System
# Author: WilisBS, AdhiS, GhiffaroNR, TuahtaR, Brillian 
Question answering system (for text in Bahasa Indonesia) using nltk CRFTagger, nltk StanfordNERTagger, Sastrawi (for text preprocessing), and simple weighting (similar words).

1. you have to know first the differences between pos-tag and ner-tag

*Text Preparation

2. prepare text data
3. make CRFTagger Model manually based on the text data
4. download Stanford NER Tagger package (Indonesia)
5. text preprocessing 
6. create CRFTagger method
7. create StanfordNERTagger method

*Question processing

8. generate question-word from question
9. divide the type of every question-word (postag/nertag)
10. generate type of answer-tag (postag/nertag) based on question-word
11. preprocessing question (used as keyword)
12. apply CRFTagger to the question
13. generate verb from question

*Text weighting

14. split text as passage
15. simple weigting proccess using similar words between every passage and keyword (from question)
16. retrieve passage with the highest weight 

*Answer Processing

17. generate type of answer-tag (from question processing)
18. apply CRFTagger/StanfordNERTagger to the retrieved passage (based on type of answer-tag)
19. get the answer from passage with the same tag as the answer-tag
20. verb (from question) is only used if the question-word is "apa" (what)
