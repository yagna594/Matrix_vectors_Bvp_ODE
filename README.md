# Matrix_vectors_Bvp_ODE libraries

Developing Matrix Class for Linear Algebra
Calculations

• Develop a class of matrices called Matrix for use with the class of vectors.

• Your class implementation should include the following features: { private members mnum rows and mnum cols that are integers and store the number of rows and columns { mData that is a pointer to a double-precision floating-point variable, which stores the address of a pointer to the first entry of the first row

• A constructor that accepts two positive integers - num rows and num cols as input assigns these values to the class members mnum rows and mnum cols, allocates memory for a matrix of size mnum rows and mnum cols, and initializes all entries to zero.

• An overridden copy constructor that copies the variables mnum rows and mnum cols, allocates memory for a new matrix, and copies the entries of the original matrix into the new matrix.

• An overridden destructor that frees the memory that has been allocated to the matrix.

• Public methods for accessing the number of rows, and the number of columns.

• An overloaded round bracket operator with one-based indexing for accessing the entries of the matrix so that, provided i and j are valid indices for the matrix, A(i,j) may be used to access mData[i-1][j-1]

• Overloaded assignment, unary and binary operators to allow addition, subtraction and multiplication of suitably sized matrices, vectors and scalars. You should use assert statements to ensure the matrices and vectors are
of the correct size.

• A public method that computes the determinant of a given square matrix.

Developed a class called LinearSystem that may be used to solve linear systems. Assuming the system is nonsingular, a linear system is defined by the size of the linear system, a square matrix, and a vector (representing the right-hand side), with the matrix and vector being of compatible sizes. The data associated with this class may be specified through an integer variable mSize, a pointer to a matrix mpA, and a pointer to the vector on the right-hand side of the linear system mpb.


We suggest only allowing the user to set up a linear system through the use of a constructor that requires specification of the matrix and vector: the member mSize may then be determined from these two members. If you do not wish to provide a copy constructor, the automatically generated copy constructor should be overridden and made private to prevent its use. As with the class of vectors, we recommend the use of the automatically generated default constructor is prevented by providing a specialised constructor but no default constructor.
A public method Solve should be written to solve this linear system by Gaussian elimination with pivoting. This method should return a vector containing the linear system's solution. You should be able to test your class using the appropriate examples. You might want to consider the following to test your class implementation:

• test the various constructors.

• test solving problems when the matrix is poorly conditioned.

• test that the Gaussian Elimination routine performs pivoting when small values appear on the diagonal.

• test various Matrix and Vector methods.

