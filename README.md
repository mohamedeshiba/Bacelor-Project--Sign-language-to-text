# Bacelor-Project--Sign-language-to-text
Sign language is known to be the way that hearing-impaired people use to communicate with other people in the community. They use their hands' gestures to represent a word or an expression. There was always a need to some interpreter who is familiar with the different signs, that's why there are many recent studies on how to make disabled people communicate
more easily. This study aims to develop a real-time \acf{ASL} recognition system for people who do not know sign language rules to communicate easily
with hearing-impaired people. We focused on making the recognition system for dynamic signs that requires hand movement instead of static signs. Our proposed solution is to use \acf{RNN}, \ac{LSTM} model, to train it on a data-set of some common signs in the \ac{ASL}. Due to the shortage of an open-source dynamic data-set, We created our own data-set for 7 expressions each one with 30 videos (variations) where each video consists of 30 frames to fully represent the hand movement. In the feature extraction step, we used \acf{MP} frame work provided by google to detect the hands and the face accurately and efficiently. MediaPipe represent the features as extracted landmarks in each frame. The extracted landmarks from each video were concatenated together in a numpy array. Each video was labelled and fed to the model to be trained on. We tried two different approaches on the shape of the data fed to the model and evaluated both of them. The performance of the proposed system has also been evaluated on the basis
of confusion matrix, accuracy, precision, recall and f-score.  
The training accuracy reached 100\% and the testing accuracy reached 85.71\%, while the model achieved F1-score of 85.87\%. The system can be enhanced in the future by extending the data-set to hold large number of expressions with different variations on different set of people.
