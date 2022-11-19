# AdvAlgo_Raga
1. Title of the Project: Carnatic Raga Identifier
2. Problem Statement: Using Machine Learning and Deep Learning algorithms to identify
the Carnatic Raga of given audio test file.
3. Motivation:
Listening to a given audio/music recording and identifying the Carnatic Raga it belongs
to is part of the routine for a music student. Being a student of Carnatic Music for the past
15+ years, and after getting introduced to the fields of ML and DL through Engineering,
it was only intuitive for me to try to implement the idea of training machine to identify
the ragas.
A student, after years of listening, knowledge of each raga, a lot of muscle memory can
identify ragas. I thought it would be a good challenge and more importantly, a great
learning opportunity for me to test my skills, gain knowledge and hopefully, help many
other music students in their journey!
4. References and Related Research:
• The Youtube lecture series by “Valerio Velardo” titled “Audio Signal Processing
for Machine Learning” was very helpful in introducing the basics and concepts of
Audio Signal Processing for ML and working with audio files, features in python.
• Music Information Retrieval: Raga Identification using Machine Learning (IIT
Madras):
https://www.iitm.ac.in/donlab/website_files/thesis/MTech/thesis_padma.pdf
https://publications.iitm.ac.in/publication/classification-of-melodic-motifs-inraga-music-with-time-series-2
• Raga Identification using ML: https://medium.com/@shreyas.divan/ragaidentification-using-ml-and-dl-a95b51f47044
• https://www.linkedin.com/pulse/identifying-ragas-carnatic-music-machinelearning-sridhar-ravikoti/
5. Approach:
Considering there are 1000+ identifiable ragas in Carnatic Music, I have only considered
2 ragas i.e., Thodi and Kambodi. The objective of this program is to classify a given test
audio as belonging to either of the above mentioned two ragas (for purpose of this
project, during the prediction phase, test audio strictly belonging to either raga only is
chosen).
Data Collection: To train the models, I have chosen about 10 recordings consisting a
mixture of vocal (female and male) and instrumental audio files.
Data Preparation: All files are converted to wav format so that they can be loaded using
librosa module of python. The user-defined function converts the training audio files into
snippets of 10 seconds, with the specified jump.
Next, features from these snippets are extracted using the various built-in functions of
librosa module (Mel Spectogram, MFCCs, Spectogram, Fourier Transform).
6. Unique contribution / Implementation:
I have compared the accuracies of the following ML models:
• Logistic Regression
• SVM (rbf)
• XGBoost
DL Models:
• DNNs
• LSTMs
Apart from trying to combine Deep Learning techniques along with the Machine
Learning algorithms to obtain higher accuracy in predicting the ragas of test audio files, I
have recorded my own audio files to assist in training the models.
7. System Architecture, Design and Implementation:
I have created 4 folders (thodi_test, kambodi_test, thodi_training and kambodi_training)
which contain the required audio files to train and test the models.
Tweaking the following individual parameters of DNN model was observed to produce
the best predictions:
• Optimizer
• Learning Rate
• Batch Size
• Number of deep layers, etc
Once the training process was done, random train-test splitting method of sklearn module
was made use of, to generate completely random audio files and test the trained models
for their accuracy of predictions.
8. Analyzing the Results:
• Accuracy on test data for ML classifiers: (Output form ipynb file)
• Accuracy obtained when DNN used:
• Prediction on unknown test audio file using ML classifier:
• Final predictions of 16 audio files:
9. Conclusion:
From the above results, we observe that among the ML classifiers:
LR(80%) > XGB (~65%) > SVM (~66%)
While using DL, we achieved an accuracy of ~70%
Hence, considering the quality of used training data and test cases used to predict and
calculating the accuracy, we have achieved 80% accuracy in predicting the raga for a
random audio test file.
With further improvements in the training audio files and a better dataset, using more
specific test data, higher accuracies can be achieved.
10. Future Work:
I plan to further expand the scope of the raga identifier, by including more ragas and
trying to improve the accuracy too.
Furthermore, we can use the same algorithm to use ML and DL algorithms to recognize
the voice of the performer. These can be used as an innovative kind of biometrics to
lock/unlock digital devices, which recognize the voice of the authorized user only.
Link to the GitHub Repo: https://github.com/GovindaMadhava/AdvAlgo_Raga
