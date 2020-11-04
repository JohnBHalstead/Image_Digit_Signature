# Image_Digital_Signature
Improved jupyter notebook Python code for creating a classifier that recognizes the image digit of five as presented in Geron's 2nd edition "Hands-on Machine Learning with Scikit-Learn, Keras, and TensorFlow".

This real basic prototype creates a signature for the digital image of 5 in the publicly available MNIST data.
 
I ran two classifiers on the feature and flag pairs. For one classifier (Stochastic Gradient Descent), I include five evaluation methods: Confusion Matrix, two Precision and Recall graphs, a ROC curve, and an AUC. For the other classifier (Random Forest) I just used a ROC and AUC. The Random Forest outperformed the SGD for these data. The SGD AUC was approximately 0.96, while the RF was 0.99.
 
The “trick” with creating a signature concerns the label’s transformation. It’s really basic. It involves pairing a feature set with a binary response. Flags are one for the desired signature and zero for all others.  In application, a model would have to be trained for each desired signature. In this case the classification tasks are for images ranging from 0 to 9. Ten models are required. In the example, a signature was created for the digital image of 5.
 
The MNIST data are a collection of digit images handwritten by high school students and employees of the US Census Bureau. The data are conveniently randomized into a training and test data sets. The first 60K are training data and the last 10K are test data.
 
The code is expanded and improved from the examples Geron provides in his Chapter 3 of “Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems, 2nd Edition”, O’Reilly, Boston MA, USA 2019.
 
