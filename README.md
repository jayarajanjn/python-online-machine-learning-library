# python-online-machine-learning-library

## Description

This is a python online machine learning library (POMLL) for some famous classifiers.  
The following classifiers are implemented.

* Passive Agrressive Algorithm  
    * L1-hinge loss  
    * L2-hinge loss  
* Confidence Weighted  
    * variance version  
* Multi-Class Multi-Label Confidence Weighted   
    * single contraint and diagonal matrix version  
* Adaptive Regularization of Weights  
    * dense matrix  
    * diagonal matrix  
* Softconfidence Weighted  
    * L1-hinge loss  
    * L2-hinge loss  
* Softconfidence Weighted  
    * L1-hinge loss, single contraint, and diagonal matrix  
* L2-hinge loss, single contraint, and diagonal matrix  
* Logistic Regression (should not be used)  
    * solved with stochastic gradient  

## Dependency
* numpy
* (scipy)
* (scikit-learn)

## How to use
Refer to the main function and and class method, examplify.

## Data Format
* Dense Matrix  
    * label,d1,d2,...,dn
    * example for binary  
        1,0.1,0.2, ...,0.9  
        2,0.1,0.2, ...,0.9  
        ...  
        1,0.1,0.2, ...,0.9  
        2,0.1,0.2, ...,0.9  

    * example for multi-class  
        1,0.1,0.2, ...,0.9  
        2,0.1,0.2, ...,0.9  
        ...  
        3,0.1,0.2, ...,0.9  
        2,0.1,0.2, ...,0.9  

## Note
* All labeled samples to be used for learning are included in memory.
* Dense matrix format (2-dimensional ndarray) are used now.
* All algorithm except for Multi-Class Multi-Label CW and SCW are for binary classification only.
* A sample is normalized such that the norm of sample is equal to 1.
* Bias, 1 is added to a sample.

## References
* http://webee.technion.ac.il/people/koby/publications/arow_nips09.pdf
* http://www.aclweb.org/anthology/D/D09/D09-1052.pdf
* https://alliance.seas.upenn.edu/~nlp/publications/pdf/dredze2008f.pdf
* http://webee.technion.ac.il/people/koby/publications/paper_nips08_std.pdf
* http://icml.cc/2012/papers/86.pdf

## Future Work
* Sparse matrix is used.
* Binary classifiers are extended to 1-vs-n and/or pair-wise classifiers.
* All labeled samples to be used for learning are not necessarily included in memory.

