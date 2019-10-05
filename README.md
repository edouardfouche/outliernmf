# outliernmf
This is the matlab implementation for the paper titled "Outlier Detection for Text Data"

* Generate a labelled dataset with 0 as non-outliers and 1 as outliers.
* Call the textoutliers function with the sparse bag of words matrix, low rank k, parameters alpha and beta.
* It will return three matrices Z,W,H.
* Use L2 score of every column of Z as the outlier score for every document.
* Call ROC curve module with L2 score of every column of Z against the labels from step 1.
* The code is tested with MATLAB R2011b (MATLAB 7.13). It should also work with any later versions. It must also work fine with octave

## Reproducing the experiments

Currently, I am trying to reproduce the experiments from the paper, in particular, against the Reuters and RCV20 data set. To reproduce the experiments, you may run the `reproduce.ipynb` notebook (see the comments therein). 
However, for some reason I am not getting the results claimed in the paper. 

## Citation ##
* Ramakrishnan Kannan, Hyenkyun Woo, Charu C. Aggarwal and Haesun Park. "Outlier Detection for Text Data", Accepted at 2017 International Conference on SIAM Data Mining 

