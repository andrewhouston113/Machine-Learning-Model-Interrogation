# Machine-Learning-Model-Interrogation


## Contents

- [Overview](#overview)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
- [License](#licencse)
- [Citation](#citation)


## Overview
A tutorial for interrogating the performance of machine learning models using hardness measures and difficulty-based incremental evaluations. 

In this tutorial, we will go step-by-step throught a model interrogation process that:

1.   Characterises an instances difficulty using a simple instance hardness metric representative of the likelihood an instance will be misclassified
2.   Calculates 4 hardness measures, each representing a source of difficulty from a data perspective
3.   Performs a correlational analysis that identifies which measure most relates to misclassifications within the current task
4.   Identifies which model best handles the source of difficulty associated with misclassifications 

The resources used in generating this code were:

M. R. Smith and T. Martinez, "Improving classification accuracy by identifying and removing instances that should be misclassified," The 2011 International Joint Conference on Neural Networks, 2011, pp. 2690-2697, doi: https://doi.org/10.1109/IJCNN.2011.6033571

Smith, M.R., Martinez, T. & Giraud-Carrier, C. An instance level analysis of data complexity. Mach Learn 95, 225–256 (2014). https://doi.org/10.1007/s10994-013-5422-z



## System Requirements

### OS Requirements
The code development version has been test on Windows operating systems. The code is provided as a .ipynb and can be run on Google Colab and should in theory work on any operating system.

### Installation Guide
#### Dependencies
Installation should not be required for Google Colab, hoever, should the users not be using Google Colab, the following dependencies should be installed (installation of all packages should take no longer than 5 minutes):

```
pandas 1.1.5
numpy 1.19.5
matplotlib 3.2.2
sklearn 0.22.2
mpl_toolkits 1.2.1
scipy 1.4.1
```
## Instructions for Use
A tutorial has been provided withing the .ipynb on a simulated dataset. To apply the interrogation procedure to your own dataset simply replace the generated X and y with your dataset, and replace the predictions and probabilites with those genetated by you own models. X should take the form of an m x n matrix where m is the number of samples and n is the number of features, y should be an array of length m, containing the ground truth labels. Predictions and Probabilities should be an m x l matrix, where m is the number of samples (indexed identically to X and y) and l is the classification predictions and probabilites for each tested model. In the tutorial we have used four classifiers: Logistic Regression, Linear-SVM, KNN and Random Forest. The time taken to run the code should be no more than 5 minutes.

## Citation
Should you use this model interrogation in your work please cite the following:

```
Houston, AD., Cosma, G., Turner P., Bennett AN. (2021). Predicting surgical outcomes for chronic exertional compartment syndrome using a machine learning framework with embedded trust by interrogation strategies. Sci Rep 11, 24281 (2021). https://doi.org/10.1038/s41598-021-03825-4

```

## License
Copyright 2021 Andrew David Houston

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
