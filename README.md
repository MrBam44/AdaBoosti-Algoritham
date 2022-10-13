# AdaBoosti-Algoritham
An intuitive explanation of AdaBoost algorithn
AdaBoost recap
Let Gm(x) m=1,2,...,M be the sequence of weak classifiers, our objective is to build the following:

G(x)=sign(α1G1(x)+α2G2(x)+...αMGM(x))=sign(∑m=1MαmGm(x))
The final prediction is a combination of the predictions from all classifiers through a weighted majority vote

The coefficients αm are computed by the boosting algorithm, and weight the contribution of each respective Gm(x). The effect is to give higher influence to the more accurate classifiers in the sequence.

At each boosting step, the data is modified by applying weights w1,w2,...,wN to each training observation. At step m the observations that were misclassified previously have their weights increased
Note that at the first step m=1 the weights are initialized uniformly wi=1/N
