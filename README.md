# Machine-Learning-Model-Interrogation
A tutorial for interrogating the performance of machine learning models using hardness measures and difficulty-based incremental evaluations. 

In this tutorial, we will go step-by-step throught a model interrogation process that:

1.   Characterises an instances difficulty using a simple instance hardness metric representative of the likelihood an instance will be misclassified
2.   Calculates 4 hardness measures, each representing a source of difficulty from a data perspective
3.   Performs a correlational analysis that identifies which measure most relates to misclassifications within the current task
4.   Identifies which model best handles the source of difficulty associated with misclassifications 
