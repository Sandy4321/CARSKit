# CARSKit

### Introduction

**CARSKit** (https://github.com/irecsys/CARSKit/) is an open-source Java-based recommendation engine, where it can be used, modified and distributed under the terms of the GNU General Public License. (Java version 1.7 or higher required). It is specifically designed for context-aware recommendations. 

### Architecture and Design

![CARSKit Structure](http://students.depaul.edu/~yzheng8/images/CARSKit.png)

### Algorithms

* **Traditional recommendation algorithms**: The implementations of those algorithms (such as UserKNN, BiasedMF, SVD++, SLIM, etc) are from LibRec-V1.3. Those algorithms can be used in two ways: 1). run a traditional recommendation algorithm directly on the context-aware data set to compete with the context-aware recommendation algorithms; 2). run contextual recommendation algorithms based on transformation, e.g., run a traditional recommendation algorithms after data transformation (e.g., by item splitting).
* **Context-aware recommendation algorithms**: CARSKit simply divides it into two categories: Transformation Algorithms and Adaptation Algorithms. The transformation algorithms try to convert the mulidimensional recommendation problem into traditional 2-dimensional problem, so that the traditional recommendation algorithms can still be used. In contrast to those algorithms based on transformation algorithms, the adaptation algorithms focus on their effect on building algorithms by adapting to the multidimensional rating space. Most of the algorithms inside belong to the contextual modeling algorithms, such as Context-aware Matrix Facatorization, Tensor Factorization, Contextual Sparse Linear Method, Factorization Machines, and so forth.

### Reference

Please cite the following papers if you use CARSKit in your research:

1. Yong Zheng, Bamshad Mobasher, Robin Burke. "CARSKit: A Java-Based Context-aware Recommendation Engine", Workshop Proceedings of the 15th IEEE International Conference on Data Mining (ICDM 2015), Atlantic City, NJ, USA, Nov 2015

### Data Sets

A list of context-aware data sets can be found here: http://tiny.cc/contextdata <br/>
Please consider filling out our survey on movie ratings: http://tinyurl.com/surveycars

### Acknowledgement

I would like to show our gratitude to Dr. Guibing Guo (the author of LibRec) for his comments and suggestions on the development of CARSKit.

### Release Notes

**2015/08/25, Pre-Release**

Most algorithms (traditional recsys algorithms and context-aware recsys algorithms) have been implemented. Only a few of more changes will be made, and probably some new CARS algorithms (published in 2015) will be implemented. API documents will be created, as well as a short demo. The CARSKit is almost done, and it will be released in September, 2015, estimatedly.







