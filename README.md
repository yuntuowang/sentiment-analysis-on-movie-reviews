# sentiment-analysis-on-movie-reviews
This project is based on https://github.com/rafacarrascosa/samr/tree/develop/samr.

Based on the current code, the valid values of the main classifier used are “sgd”(SGDClassifier),
“knn”(KNeighborsClassifier), “svc”(SVC), and “randomforest”(RandomForestClassifier).

Corresponding to each classifier, there is a dictionary to be passed as arguments. 
And we can also use other classifiers by importing them, as long as they have been implemented in scikit-learn library.

Basically, I created several json file containing the differnet arguments of different classifiers, 
compare their performances and analyze the reasons. Based on the scikit-learn documentations, I analyzed the effects of arguments.
Note that SVM training can be arbitrary long, this depends on dozens of parameters:
C parameter - greater the misclassification penalty, slower the process; kernel - more complicated the kernel, slower the process
(rbf is the most complex from the predefined ones); 
data size/dimensionality - again, the same rule.

Within the scope I have experimented, "randomforest" performs best in this case.
