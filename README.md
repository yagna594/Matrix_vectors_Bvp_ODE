# Matrix_vectors_Bvp_ODE libraries

Developing Matrix Class for Linear Algebra
Calculations

• Develop a class of matrices called Matrix for use with the class of vectors.
• Your class implementation should include the following features: { private members mnum rows and mnum cols that are integers and store the number of rows and columns { mData that is a pointer to a double-precision floating-point variable, which stores the address of a pointer to the first entry of the first row
• A constructor that accepts two positive integers - num rows and num cols as input assigns these values to the class members mnum rows and mnum cols, allocates memory for a matrix of size mnum rows and mnum cols, and initializes all entries to zero.
• An overridden copy constructor that copies the variables mnum rows and mnum cols, allocates memory for a new matrix, and copies the entries of the original matrix into the new matrix.
• An overridden destructor that frees the memory that has been allocated to the matrix.
• Public methods for accessing the number of rows, and the number of columns.
• An overloaded round bracket operator with one-based indexing for accessing the entries of the matrix so that, provided i and j are valid indices for the matrix, A(i,j) may be used to access mData[i-1][j-1]
• Overloaded assignment, unary and binary operators to allow addition, subtraction and multiplication of suitably sized matrices, vectors and scalars. You should use assert statements to ensure the matrices and vectors are
of the correct size.
• A public method that computes the determinant of a given square matrix.

