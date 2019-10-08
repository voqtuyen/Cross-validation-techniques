# Guideline to data splitting in machine learning


Suppose we want to train a supervised learning model on the dataset T = {<a href="https://www.codecogs.com/eqnedit.php?latex={(x^{1},y^{1}),&space;(x^{2},y^{2}),...,(x^{m},y^{m})}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?{(x^{1},y^{1}),&space;(x^{2},y^{2}),...,(x^{m},y^{m})}" title="{(x^{1},y^{1}), (x^{2},y^{2}),...,(x^{m},y^{m})}" /></a>}. 
At the end of the training process, the final model should predict correct outputs for the input samples from T, but it should also be able to generalize well to previously unseen data.

Generalization refers to your model's ability to adapt properly to new, previously unseen data, *drawn from the same distribution* as the one used to create the model [9]. Poor generalization is maily caused by overfitting and underfitting. If the model is overfitting, it just memorizes the training examples and it is not able to give correct outputs also for examples that were not in the training set. On the contrary, if the model is underfitting, it does not perform well on the training examples as well as for examples that are not in the training set.

Cross-validation techniques are used to ensure good generalization and to avoid overfitting. The basic idea is to divide the dataset T into two subsets – one subset is used for training while the other subset is left out and the performance of the final model is evaluated on it. Cross-validation techniques could be used for model selection and performance estimation
- Model selection
- Performance estimation

## Reference

1. https://www.mff.cuni.cz/veda/konference/wds/proc/pdf10/WDS10_105_i1_Reitermanova.pdf
2. https://developers.google.com/machine-learning/crash-course/training-and-test-sets/splitting-data
3. https://neuro.cs.ut.ee/wp-content/uploads/2015/05/BNNI2015-MLPipeline-exercise.pdf
4. https://www.mimuw.edu.pl/~son/datamining/DM/eval-train-test-xval.pdf
5. http://research.cs.tamu.edu/prism/lectures/iss/iss_l13.pdf
6. http://www.coli.uni-saarland.de/~crocker/Teaching/Connectionist/lecture11_4up.pdf
7. https://stats.stackexchange.com/questions/52274/how-to-choose-a-predictive-model-after-k-fold-cross-validation
8. https://datascience.stackexchange.com/questions/13960/how-to-choose-a-classifier-after-cross-validation/13964
9. [Machine learning crash course](https://developers.google.com/machine-learning/crash-course/generalization/video-lecture#targetText=Generalization,used%20to%20create%20the%20model.&targetText=Divide%20a%20data%20set%20into%20a%20training%20set%20and%20a%20test%20set)
