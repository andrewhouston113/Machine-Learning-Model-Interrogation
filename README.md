# Machine-Learning-Model-Interrogation
A tutorial for interrogating the performance of machine learning models using hardness measures and difficulty-based incremental evaluations. 

In this tutorial, we will go step-by-step throught a model interrogation process that:

1.   Characterises an instances difficulty using a simple instance hardness metric representative of the likelihood an instance will be misclassified
2.   Calculates 4 hardness measures, each representing a source of difficulty from a data perspective
3.   Performs a correlational analysis that identifies which measure most relates to misclassifications within the current task
4.   Identifies which model best handles the source of difficulty associated with misclassifications 

The resources used in generating this code were:

M. R. Smith and T. Martinez, "Improving classification accuracy by identifying and removing instances that should be misclassified," The 2011 International Joint Conference on Neural Networks, 2011, pp. 2690-2697, doi: https://doi.org/10.1109/IJCNN.2011.6033571

Smith, M.R., Martinez, T. & Giraud-Carrier, C. An instance level analysis of data complexity. Mach Learn 95, 225–256 (2014). https://doi.org/10.1007/s10994-013-5422-z
