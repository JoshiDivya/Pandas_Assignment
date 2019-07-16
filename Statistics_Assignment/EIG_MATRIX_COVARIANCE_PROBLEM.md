
## EigenValue Problem
 ### if there is a matrix A then the eigenvalue of matrix is λ if and only if
 * det(λIn - A) =0 satisfied 
 * A is n*n matrix
 1.Multiply an n*n identity matrix by the scalar $\lambda$.<br>
2.Subtract the identity matrix multiple from the matrix A.<br>
3.Find the determinant of the matrix and the difference.<br>
4.Solve the values of X that satisfy the equation def(A-$\lambda$I)=$\bar{0}$ .<br>
5.Solve for the corresponding vector to each $\lambda$.<br>

_Example to find Eigen Value__<br>

\begin{equation*} A = \begin{bmatrix} 2 & 3 \\ 2 & 1 \end{bmatrix} \end{equation*}

$$A - \lambda I ={\begin{bmatrix} 2 & 3 \\ 2 & 1 \end{bmatrix}} - {\begin{bmatrix} \lambda & 0 \\ 0 & \lambda \end{bmatrix}} $$

$$ ={\begin{bmatrix} 2 - \lambda & 3 \\ 2 & 1 -\lambda \end{bmatrix}} $$


(5)   \begin{equation*} Det\begin{pmatrix}2-\lambda&3\\2&1-\lambda\end{pmatrix}=0. \end{equation*}

Calculating the determinant gives:

(6)   \begin{align*} &(2-\lambda)(1-\lambda) - 6 = 0\\ \Rightarrow &2 - 2 \lambda - \lambda - \lambda^2 -6 = 0\\ \Rightarrow &{\lambda}^2 - 3 \lambda -4 = 0. \end{align*}

To solve this quadratic equation in \lambda, we find the discriminant:

   \begin{equation*} D = b^2 -4ac = (-3)^2 -4*1*(-4) = 9+16 = 25. \end{equation*}

Since the discriminant is strictly positive, this means that two different values for \lambda exist:

(7)   \begin{align*} \lambda _1 &= \frac{-b - \sqrt{D}}{2a} = \frac{3-5}{2} = -1,\\ \lambda _2 &= \frac{-b + \sqrt{D}}{2a} = \frac{3+5}{2} = 4. \end{align*}

We have now determined the two eigenvalues \lambda_1 and \lambda_2. Note that a square matrix of size N \times N always has exactly N eigenvalues, each with a corresponding eigenvector. The eigenvalue specifies the size of the eigenvector.


```python

```
