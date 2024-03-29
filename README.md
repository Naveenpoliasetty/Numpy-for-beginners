# Introduction to Numpy
<br>
NumPy, short for Numerical Python, is a fundamental package for scientific computing in Python. It provides support for large, multi-dimensional arrays and matrices, along with a collection of high-level mathematical functions to operate on these arrays. NumPy is a cornerstone library in the Python data science ecosystem and is widely used for numerical and mathematical operations.<br>

### Key Features:
#### 1. N-dimensional Arrays:
NumPy introduces the numpy.ndarray class, commonly known as arrays, which are efficient containers for large datasets. These arrays can be one-dimensional, two-dimensional, or even multi-dimensional. They provide a flexible way to represent and manipulate numerical data.

#### 2. Mathematical Operations:
NumPy offers a variety of mathematical functions that operate element-wise on arrays, making it easy to perform operations like addition, subtraction, multiplication, and more. These operations are implemented in C and Fortran, ensuring high performance.

#### 3. Broadcasting:
NumPy's broadcasting feature allows operations between arrays of different shapes and sizes. This simplifies code and eliminates the need for explicit loops, making it easier to work with arrays of varying dimensions.

#### 4. Universal Functions (ufuncs):
NumPy includes a set of universal functions, or ufuncs, which are functions that operate element-wise on arrays. These functions are optimized for performance and can be applied to entire arrays without the need for explicit looping.

#### 5. Linear Algebra:
NumPy provides a comprehensive set of linear algebra functions, including matrix multiplication, eigenvalue decomposition, and singular value decomposition. This makes it a powerful tool for a wide range of scientific and engineering applications.

#### 6. Integration with Other Libraries:
NumPy seamlessly integrates with other Python libraries, such as SciPy, pandas, and scikit-learn, creating a powerful ecosystem for scientific computing and data analysis.


## Section 1

#### 1. Creating NumPy Arrays
NumPy arrays are the foundation for numerical computing in Python. You can create an array by converting a Python list or tuple using the numpy.array function.

#### 2. Multidimensional Arrays
NumPy supports multidimensional arrays, allowing you to work with matrices and higher-dimensional data structures:

#### 3. Choice Arrays
Choice arrays refer to arrays that you explicitly set with specific values. This includes arrays filled with zeros, ones, or any constant value. These types of arrays are useful as a starting point for further operations or when you need an array with a specific initial state.

#### 4. Random Arrays
Random arrays are arrays where the elements are generated using random values. This is often used for tasks like simulations, random sampling, or creating datasets for testing and analysis. NumPy provides various functions for generating random arrays, including uniform distributions, normal distributions, and more.

#### 5. Array of Zeroes
An array filled with zeros is a convenient way to create an array where all elements have an initial value of zero. This is useful when you want to initialize an array before populating it with actual data.

#### 6. Array of Ones
Similar to the array of zeroes, an array filled with ones is used when you want to initialize an array with all elements having an initial value of one. This is commonly employed when you are planning to incrementally build up the array during further computations.

#### 7. Identity Matrix Arrays
Identity matrix arrays are square matrices with ones on the main diagonal and zeros elsewhere. They play a crucial role in linear algebra operations, such as solving systems of linear equations and finding inverses.

#### 8. Evenly Spaced Arrays and Linspace Arrays
Evenly spaced arrays refer to arrays where the elements are equally spaced between a start and end value. The linspace function in NumPy is particularly useful for creating arrays with a specified number of evenly spaced values within a given range. This is often used in plotting and numerical analysis.

Understanding these different types of arrays provides a solid foundation for working with NumPy and performing a wide range of numerical computations. Feel free to delve deeper into each concept and explore their applications in various scientific and engineering scenarios.


## Section 2

#### Shaping Arrays:
Shaping arrays in NumPy refers to changing the dimensions of an array. You can use the numpy.shape attribute to get the current shape of an array, which returns a tuple representing the size of each dimension.

#### Reshaping Arrays:
Reshaping arrays involves changing the structure of an array by modifying its shape. The numpy.reshape function allows you to specify the desired new shape of the array. It's important to note that the total number of elements in the reshaped array must remain the same as in the original array.

#### Flattening Arrays:
Flattening an array means converting a multi-dimensional array into a one-dimensional array. This can be achieved using the numpy.flatten method or by calling the numpy.ravel method. The resulting flattened array retains the order of elements from the original array.

#### Raveling Arrays:
Raveling is a concept similar to flattening, where a multi-dimensional array is converted into a one-dimensional array. The numpy.ravel function is used for this purpose. It returns a flattened view of the original array whenever possible. Unlike flatten, ravel may return a reference to the original data if no copy is needed.

## Section 3

#### Slicing 2D and 3D Arrays
Slicing in 2D Arrays:
Slicing involves extracting specific portions of an array. In 2D arrays, you can slice along both rows and columns using indexing. For example, array[row_start:row_end, col_start:col_end] extracts a subarray from the original array.

Slicing in 3D Arrays:
Slicing extends naturally to 3D arrays, allowing you to select specific elements along each dimension. Slicing in 3D involves specifying ranges for the three dimensions, such as array[depth, row_start:row_end, col_start:col_end].

#### Negative Slicing:
Negative indexing allows you to slice arrays from the end. For instance, array[:, -3:] selects the last three columns of a 2D array.

#### Stacking Arrays
Vertical Stacking:
Vertical stacking, or numpy.vstack, combines two or more arrays vertically along the first axis. This is useful when you want to concatenate arrays with the same number of columns.

#### Horizontal Stacking:
Horizontal stacking, or numpy.hstack, concatenates arrays side by side along the second axis. This is beneficial when combining arrays with the same number of rows.

#### Depth Stacking:
Depth stacking, or numpy.dstack, stacks arrays along the third axis. This is primarily used for 3D arrays.

#### Concatenating Arrays
Vertical Concatenation:
Vertical concatenation, or numpy.concatenate with axis=0, joins arrays along the first axis, effectively stacking them vertically.

Horizontal Concatenation:
Horizontal concatenation, or numpy.concatenate with axis=1, concatenates arrays along the second axis, resulting in a wider array.

## Section 4

#### Splitting Arrays
Vertical Splitting
Vertical splitting divides an array into multiple subarrays along the vertical axis, which corresponds to the rows of the array. This operation is useful when you want to break down a large array into smaller, vertically aligned segments. You can specify the number of subarrays or provide a list of indices to determine where the splits should occur along the rows.

Horizontal Splitting
Horizontal splitting, on the other hand, divides an array into multiple subarrays along the horizontal axis, corresponding to the columns of the array. This is helpful when you want to segment an array into smaller, horizontally aligned chunks. Similar to vertical splitting, you can specify the number of subarrays or provide a list of indices to determine where the splits should occur along the columns.


