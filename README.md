# illness-svm-naive-bayes

# Description of Analysis Conducted

-For Mr. John Hughes, we are conducting the analysis where we are building and evaluating two models based on the data which consists of 30 attributes for tumor measurement and 1 variable indicating the diagnosis done.
-We will be carrying out analysis based on two models i.e. Support Vector Machines and Naïve Bayes.
-Support Vector Machines take the classification approach and can be used in regression analysis as well. Basically here, the classification is done by putting a hyperplane to separate two or more variables which creates a margin.
-Naïve Bayes is based on Bayes Theorem and the probability of having a strong (Naïve) independent assumptions between the features.

# Summary of Analysis

-In the analysis done, the first step we do is to import necessary libraries, i.e. pandas, numpy, and matplotlib.
-Next is we load the dataset provided, “illness.csv”.
-As we print the head of the dataset (first 5 rows) we see that the first 30 columns depict the tumor measurement variables, (independent) and the last columns depicts the diagnosis which can be either M (Malignant) or B (Benign) which is the dependent variable.
-After this, we set up the dependent and independent variables and split the data into training and testing data.
-We further scale the data; all of this is carried out by using the scikit-learn library.
-Now we set up our models on the data, by mentioning the random state to 100 and target names to be “B” and “M”.
-We can see that we have a confusion matrix provided for both SVM and Naïve Bayes models.
-Now, the comparison, evaluation, and decisions can be made by obtaining this output.

# Compare the SVM Algorithm to the Naïve Bayes Algorithm

-In the output obtained for both the algorithms, in SVM, the confusion matrix depicts the True Positive of SVM (69) is more than Ture Positive of Naïve Bayes (66).
-This automatically affects the False Negative of SVM (3) and False Negative of Naïve Bayes (6).
-We also see a difference in the values of precision for B (Benign) for SVM (0.93) as compared to the values of precision for B (Benign) for Naïve Bayes (0.87).
-We also see a difference in the values of recall for M (Malignant) for SVM (0.96) as compared to the values of recall for M (Malignant) for Naïve Bayes (0.92)
-We also see a difference in the values of f1-score for M (Malignant) for SVM (0.97) as compared to the values of f1-score for M (Malignant) for Naïve Bayes (0.94)
-The macro and weighted averages of both the algorithms differ from the each other, the values of SVM are higher in all.
-All these factors affect the overall accuracy on the algorithm which is 96% for SVM and 93% for Naïve Bayes.

# Important Insights

-The insights obtained from the output are that as the precision, recall, and f1-score of Malignant and Benign differ from each other very minutely, the data provided works well to an extent on both the algorithms.
-The main insight we can pick up from the confusion matrix is the similarity of False Positive and True Negative and the difference in True Positive and False Negative.
-We know its always better when the value of False Positive and False Negatives should be less and True Positive and True Negative be more.
-Weighted Averages are taken into consideration while evaluating any algorithm, here the values differ significantly for the precision, recall as well as f1-score, the same goes with the macro average.
-For all the values obtained in precision, recall, and f1-score for macro averages and weighted averages, it depicts the whole scenario where the accuracy is 96% for SVM and 93% for Naïve Bayes.

# Recommendation and Justification on model selection

-From the analysis done, it can be said that the better algorithm out of the two is Support Vector Machines.
-We can conclude choosing SVM as the values differing in the confusion matrix True Positive and False Negative can be spotted.
-The precision, recall and f1-score values also depict a huge difference and SVM gets ahead out of the two in this too.
-Also, as the weighted average being an important catalyst shows how exactly it increases 3% right from 93 to 96, which in a way shows the accuracy of the model.
-Therefore, we conclude that the better model out of the two to choose would be Support Vector Machines.
