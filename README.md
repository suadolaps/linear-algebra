#Linear Algebra Exercises
Course: [Mathematics for Machine Learning](https://www.coursera.org/courses?query=mathematics%20for%20machine%20learning "Mathematics for Machine Learning")

The linear algebra section of the course involved working on four applications:
1. **Identifying Special Matrices**: This involved writing code that allows you to change a matrix to row echelon form by applying Gaussian Elimination.

2. **Reflecting Bear**: This involved applying a transformation matrix to a vector with a non-orthonormal co-ordinate system. In the case of this assignment, I want to write a transformation matrix that for reflecting bear's vectors in his co-ordinate system. 

3. **Gram-Schmidt Process**: This involved writing a function that forms an orthonormal basis from a set of vectors. 

##[Identifying Special Matrices]()
With Gaussian elimination, we want all the numbers below the leading diagonal to be 0. This changes a matrix into row echelon form and allows us to solve systems on equation.

In this exercise, I worked on a functions that fixed each row of a 4 x 4 matrix. Before completing this exercise, I manually worked on a 4x4 matrix, changing it to row echelon form to help me visualise the process each step of the way. This made it easier to transfer my mathematical knowledge to code. 

- For row zero, it is required that the first element is 1, so this required dividing each element by the first element. 
- For row one, the first element need to be zero, and the diagonal element needs to be 1. 

This process is carried out for each of the rows, until all the elements below the leading diagonal have values of zero. 

##[Reflecting Bear]()
