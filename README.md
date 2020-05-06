# Linear Algebra Exercises
Course: [Mathematics for Machine Learning](https://www.coursera.org/courses?query=mathematics%20for%20machine%20learning "Mathematics for Machine Learning")

The linear algebra section of the course involved working on four applications:
1. **Identifying Special Matrices**: This involved writing code that allows you to change a matrix to row echelon form by applying Gaussian Elimination.

2. **Reflecting Bear**: This involved applying a transformation matrix to a vector with a non-orthonormal co-ordinate system. In the case of this assignment, I want to write a transformation matrix that for reflecting bear's vectors in his co-ordinate system. 

3. **Gram-Schmidt Process**: This involved writing a function that forms an orthonormal basis from a set of vectors. 

## [Identifying Special Matrices](https://github.com/suadolaps/linear-algebra/blob/master/IdentifyingSpecialMatrices.ipynb)
With Gaussian elimination, we want all the numbers below the leading diagonal to be 0. This changes a matrix into row echelon form and allows us to solve systems on equation.

In this exercise, I worked on a functions that fixed each row of a 4 x 4 matrix. Before completing this exercise, I manually worked on a 4x4 matrix, changing it to row echelon form to help me visualise the process each step of the way. This made it easier to transfer my mathematical knowledge to code. 

- For row zero, it is required that the first element is 1, so this required dividing each element by the first element. 
- For row one, the first element need to be zero, and the diagonal element needs to be 1. 

This process is carried out for each of the rows, until all the elements below the leading diagonal have values of zero. 

## [Reflecting Bear](https://github.com/suadolaps/linear-algebra/blob/master/ReflectingBear.ipynb)
The aim of this exercise was to construct a function that returns the result of applying a transformation matrix on a vector. In this case, the transformation being applied to bear’s basis (the vector) is a reflection. As bear’s vectors are not orthonormal, the first step involved changing the basis using the Gram-Schmidt process. 

To transform a vector, r, you multiply it by the transformation matrix to obtain the new position of the vector. 

## [Gram-Schmidt](https://github.com/suadolaps/linear-algebra/blob/master/GramSchmidtProcess.ipynb)

In this exercise, I wrote a function that performs the Gram-Schmidt process on a set of four basis vectors, and using the learnings from that rule, I wrote a general function which performs the Gram-Schmidt process for an arbitrary number vectors. 

The steps include:

1. Ensuring each vector is orthogonal to the vectors before it. This is done by subtracting previous vectors from the vector being worked on to take into account any overlap.
2. The vector is then normalised (by dividing it by its modulus)

As step 1 is repeated with every vector that comes before the vector being worked on, a for-loop can be used to execute the process before the vector is normalised. 