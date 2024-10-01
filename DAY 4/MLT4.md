1.6 Principle component analysis

(1) Basis of orthogonal vectors
(2) Expression for residues after k rounds
(3) Heuristic to choose the top-k directions

In PCA there are two major components present. 1) n: no of dataset
2) no. of features 

the first component In PCA captures the most variance in the dataset 
When the number of features becomes large, the time complexity of PCA goes high.
Features in the dataset have non-linear relationships.

PCA tries to find Eigenvectors,
How can we do that, Here is a example 

To find PCA of dataset if d >> n
compute k = xtranspose * x

then find the eigenvalues of k
e values corresponding to e values 

covariance matrix is the product of matrix and transpose of the matrix whole divided by n 
