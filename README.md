# Carnatic Raga Identifier
Compare the accuracy of Machine Learning and Deep Learning algorithms to classify Carnatic Raga audios. Since there are 1000+ identifiable ragas in Carnatic Music, I have considered 2 ragas i.e., Thodi and Kambodi, the test audio strictly belonging to either raga. 

Implemented and compared the following methods: 
Machine Learning models:- • Logistic Regression • SVM (rbf) • XGBoost 
Deep Learning models:- • DNNs •LSTMs 

Results: 
Comparing results of Machine Learning classifiers: 
Logistic Regression(80%) > XGB (~65%) > SVM (~66%) 

While using DL, we achieved an accuracy of ~70%.

Overall achieved 80% accuracy in predicting the raga for a random audio test file. 

skills: Machine Learning, Deep Learning, Audio Signal Processing, Audio Feature Extraction

References and Related Research:
• The Youtube lecture series by “Valerio Velardo” titled “Audio Signal Processing
for Machine Learning” was very helpful in introducing the basics and concepts of
Audio Signal Processing for ML and working with audio files, features in python.
• Music Information Retrieval: Raga Identification using Machine Learning (IIT
Madras):
https://www.iitm.ac.in/donlab/website_files/thesis/MTech/thesis_padma.pdf
https://publications.iitm.ac.in/publication/classification-of-melodic-motifs-inraga-music-with-time-series-2
• Raga Identification using ML: https://medium.com/@shreyas.divan/ragaidentification-using-ml-and-dl-a95b51f47044
• https://www.linkedin.com/pulse/identifying-ragas-carnatic-music-machinelearning-sridhar-ravikoti/
