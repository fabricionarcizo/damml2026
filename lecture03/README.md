# Lecture #03: Mathematical Foundations for Machine Learning

This folder contains the supporting material used during **Lecture #03** of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 10 September 2026**.

## Overview

This lecture provides essential mathematical foundations crucial for understanding machine learning algorithms and techniques. All concepts are presented through interactive Jupyter Notebooks with mathematical explanations, computational implementations, and rich visualizations to build intuitive understanding of abstract mathematical concepts.

Linear algebra forms the backbone of modern data science, machine learning, and data mining. This comprehensive introduction covers vectors, matrices, and linear transformations with practical applications in data analysis.

## Learning Objectives

By the end of this lecture, students will be able to:

- Understand vector operations and their geometric interpretations
- Perform matrix operations and comprehend their computational significance
- Solve systems of linear equations using multiple methods
- Calculate eigenvalues and eigenvectors for dimensionality analysis
- Apply linear transformations for data manipulation and visualization
- Connect linear algebra concepts to real-world machine learning applications

## Content Structure

### Vector Operations and Geometry

#### 1. **Vector Addition** (`ex01_vector_addition_plot.ipynb`)

- **Learning Objectives**: Understanding vector addition as geometric translation
- **Concepts Covered**:
  - Vector representation in 2D and 3D space
  - Parallelogram law of vector addition
  - Commutative and associative properties
  - Geometric interpretation using quiver plots
- **Key Tools**: NumPy arrays, matplotlib quiver plots, vector arithmetic
- **Applications**: Force composition, displacement calculations, feature combination

#### 2. **Vector Subtraction** (`ex02_vector_subtraction_plot.ipynb`)

- **Learning Objectives**: Mastering vector subtraction and directional relationships
- **Concepts Covered**:
  - Vector difference as displacement
  - Relationship between addition and subtraction
  - Distance calculation between points
  - Geometric visualization techniques
- **Key Tools**: Matplotlib visualization, NumPy operations, geometric plotting
- **Applications**: Direction finding, relative positioning, change detection

#### 3. **Scalar Multiplication** (`ex03_scalar_multiplication_plots.ipynb`)

- **Learning Objectives**: Understanding scaling effects on vector magnitude and direction
- **Concepts Covered**:
  - Scalar multiplication properties
  - Vector scaling and direction changes
  - Unit vectors and normalization
  - Distributive properties
- **Key Tools**: Vector scaling operations, comparative visualizations
- **Applications**: Data normalization, feature scaling, amplitude adjustment

### Vector Products and Relationships

#### 4. **Dot Product Visualization** (`ex04_dot_product_plot.ipynb`)

- **Learning Objectives**: Geometric understanding of dot product and projections
- **Concepts Covered**:
  - Dot product geometric interpretation
  - Vector projections and components
  - Orthogonality and perpendicular vectors
  - Angle calculation between vectors
- **Key Tools**: Projection calculations, angle computations, geometric plotting
- **Applications**: Similarity measures, correlation analysis, orthogonality testing

#### 5. **Dot Product Calculations** (`ex05_dot_product_calculation.ipynb`)

- **Learning Objectives**: Computational mastery of dot product operations
- **Concepts Covered**:
  - Algebraic dot product formula
  - Angle calculation using dot product
  - Vector length and magnitude
  - Cosine similarity applications
- **Key Tools**: NumPy dot operations, trigonometric functions, statistical measures
- **Applications**: Feature similarity, recommendation systems, clustering algorithms

#### 6. **Cross Product in 3D** (`ex06_cross_product_plot.ipynb`)

- **Learning Objectives**: Understanding cross product and orthogonal vector generation
- **Concepts Covered**:
  - Cross product definition and properties
  - Right-hand rule and orientation
  - Area calculation using cross product
  - 3D coordinate system navigation
- **Key Tools**: 3D plotting with matplotlib, cross product calculations, surface normal computation
- **Applications**: 3D graphics, surface normal calculation, rotation axis determination

### Matrix Operations and Properties

#### 7. **Matrix Addition and Subtraction** (`ex07_matrix_addition_subtraction_plot.ipynb`)

- **Learning Objectives**: Mastering basic matrix arithmetic operations
- **Concepts Covered**:
  - Element-wise matrix operations
  - Matrix dimension compatibility
  - Visualization using color mapping
  - Associative and commutative properties
- **Key Tools**: NumPy matrix operations, heatmap visualizations, color mapping
- **Applications**: Image processing, data transformation, dataset combination

#### 8. **Matrix Multiplication** (`ex08_matrix_multiplication_plot.ipynb`)

- **Learning Objectives**: Understanding matrix multiplication and its geometric meaning
- **Concepts Covered**:
  - Matrix multiplication algorithm
  - Dimension compatibility rules
  - Linear transformation interpretation
  - Non-commutative property
- **Key Tools**: Matrix multiplication algorithms, transformation visualization
- **Applications**: Linear transformations, neural network operations, dimensionality reduction

#### 9. **Matrix Transpose** (`ex09_transpose_matrix.ipynb`)

- **Learning Objectives**: Understanding transpose operations and symmetry properties
- **Concepts Covered**:
  - Transpose definition and notation
  - Symmetric and antisymmetric matrices
  - Properties of transpose operations
  - Relationship to dot products
- **Key Tools**: Transpose operations, symmetry visualization, property verification
- **Applications**: Data table manipulation, covariance matrices, optimization problems

#### 10. **Identity Matrix** (`ex10_identity_matrix.ipynb`)

- **Learning Objectives**: Understanding the multiplicative identity in matrix algebra
- **Concepts Covered**:
  - Identity matrix definition and properties
  - Multiplicative identity behavior
  - Relationship to inverse operations
  - Special matrix properties
- **Key Tools**: Identity matrix generation, multiplication verification, property demonstration
- **Applications**: Matrix equation solving, inverse calculation, linear system analysis

#### 11. **Matrix Inverse** (`ex11_inverse_matrix.ipynb`)

- **Learning Objectives**: Computing and understanding matrix inverses
- **Concepts Covered**:
  - Inverse matrix definition and existence
  - Singularity and non-invertible matrices
  - Inverse calculation methods
  - Verification of inverse properties
- **Key Tools**: NumPy linear algebra functions, inverse computation, condition number analysis
- **Applications**: System solving, data transformation reversal, optimization methods

#### 12. **Matrix Determinant** (`ex12_determinant_matrix.ipynb`)

- **Learning Objectives**: Computing determinants and understanding their geometric meaning
- **Concepts Covered**:
  - Determinant definition and calculation
  - Geometric interpretation as scaling factor
  - Relationship to matrix invertibility
  - Cofactor expansion method
- **Key Tools**: Determinant calculation algorithms, geometric visualization
- **Applications**: Volume scaling, invertibility testing, characteristic polynomial

### Systems of Linear Equations

#### 13. **Substitution Method** (`ex13_substitution_system_equation.ipynb`)

- **Learning Objectives**: Solving linear systems using algebraic substitution
- **Concepts Covered**:
  - Substitution algorithm and steps
  - Variable elimination strategy
  - Solution uniqueness and existence
  - Computational complexity considerations
- **Key Tools**: Symbolic computation, step-by-step solution visualization
- **Applications**: Simple system solving, analytical solutions, educational demonstrations

#### 14. **Elimination Method** (`ex14_elimination_system_equation.ipynb`)

- **Learning Objectives**: Systematic elimination for linear system solutions
- **Concepts Covered**:
  - Gaussian elimination process
  - Row operations and equivalence
  - Forward and backward substitution
  - Pivot selection strategies
- **Key Tools**: Row operation visualization, elimination step tracking
- **Applications**: General system solving, numerical stability, algorithmic implementation

#### 15. **Matrix Inversion Method** (`ex15_matrix_inversion_system_equation.ipynb`)

- **Learning Objectives**: Solving systems using matrix inverse operations
- **Concepts Covered**:
  - Matrix equation formulation (Ax = b)
  - Inverse-based solution method
  - Computational efficiency considerations
  - Numerical stability issues
- **Key Tools**: Matrix inverse calculation, system solution verification
- **Applications**: Multiple right-hand sides, repeated system solving, theoretical analysis

#### 16. **Gaussian Elimination** (`ex16_gaussian_elimination_system_equation.ipynb`)

- **Learning Objectives**: Implementing systematic Gaussian elimination algorithm
- **Concepts Covered**:
  - Complete Gaussian elimination process
  - Partial and complete pivoting
  - Row echelon and reduced row echelon forms
  - Algorithm optimization techniques
- **Key Tools**: Step-by-step elimination visualization, numerical implementation
- **Applications**: Large system solving, numerical linear algebra, computational efficiency

### Advanced Matrix Concepts

#### 17. **Matrix Rank** (`ex17_rank_matrix.ipynb`)

- **Learning Objectives**: Understanding matrix rank and its implications
- **Concepts Covered**:
  - Matrix rank definition and calculation
  - Linear independence of rows/columns
  - Relationship to system solvability
  - Rank-nullity theorem
- **Key Tools**: Rank calculation algorithms, linear independence testing
- **Applications**: Dimensionality analysis, data redundancy detection, feature selection

#### 18. **Eigenvalue Calculation** (`ex18_eigenvalues_calculation.ipynb`)

- **Learning Objectives**: Computing eigenvalues and understanding their significance
- **Concepts Covered**:
  - Eigenvalue definition and characteristic equation
  - Eigenvalue computation methods
  - Relationship to matrix properties
  - Spectral properties of matrices
- **Key Tools**: Characteristic polynomial, eigenvalue algorithms, numerical computation
- **Applications**: Principal component analysis, stability analysis, vibration modes

#### 19. **Eigenvector Calculation** (`ex19_eigenvectors_calculation.ipynb`)

- **Learning Objectives**: Computing eigenvectors and eigenspaces
- **Concepts Covered**:
  - Eigenvector definition and properties
  - Eigenspace and geometric multiplicity
  - Orthogonality of eigenvectors
  - Complete eigendecomposition
- **Key Tools**: Eigenvector computation, eigenspace visualization, orthogonality verification
- **Applications**: Principal component analysis, dimensionality reduction, data compression

### Linear Transformations

#### 20. **Basic Linear Transformations** (`ex20_linear_transformations.ipynb`)

- **Learning Objectives**: Understanding geometric effects of linear transformations
- **Concepts Covered**:
  - Scaling transformations and effects
  - Rotation matrices and angle preservation
  - Reflection operations and symmetry
  - Composition of transformations
- **Key Tools**: Transformation matrices, geometric visualization, animation techniques
- **Applications**: Computer graphics, data rotation, geometric operations

#### 21. **Composition of Transformations** (`ex21_composition_transformation.ipynb`)

- **Learning Objectives**: Combining multiple linear transformations
- **Concepts Covered**:
  - Transformation composition rules
  - Order dependency in transformations
  - Combined scaling and rotation effects
  - Inverse transformation sequences
- **Key Tools**: Transformation chaining, sequential application visualization
- **Applications**: Complex geometric operations, multi-step data processing, graphics pipelines

## Educational Features

All notebooks include:

- 📐 **Mathematical Foundations** with rigorous definitions and theorems
- 🎯 **Interactive Visualizations** using matplotlib for geometric understanding
- 💻 **Computational Implementation** with NumPy and SciPy
- 📊 **Step-by-step Examples** showing calculation processes
- 🔍 **Geometric Interpretations** connecting algebra to visual understanding
- 📈 **Real-world Applications** in data mining and machine learning
- ✅ **Verification Methods** for checking computational results
- ⚠️ **Common Pitfalls** and numerical considerations
- 📝 **Comprehensive Exercises** for skill reinforcement

## Technical Requirements

- **Python 3.x** with scientific computing libraries
- **Core Libraries**: NumPy, matplotlib, SciPy
- **Optional Libraries**: SymPy for symbolic computation
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Mathematical Background**: High school algebra and basic trigonometry

## Learning Path

**Recommended sequence for building linear algebra mastery:**

### Foundation Level (Ex 1-6): Vector Operations

- Vector arithmetic → Scalar operations → Dot/Cross products

### Intermediate Level (Ex 7-12): Matrix Operations

- Matrix arithmetic → Special matrices → Determinants and inverses

### Advanced Level (Ex 13-16): System Solving

- Substitution → Elimination → Matrix methods → Gaussian elimination

### Expert Level (Ex 17-21): Advanced Concepts

- Matrix rank → Eigenanalysis → Linear transformations → Compositions

Each section builds essential skills needed for understanding data mining algorithms, principal component analysis, and machine learning mathematics.

## Mathematical Prerequisites

### Recommended Background

- **Algebra**: Basic algebraic manipulation and equation solving
- **Geometry**: Coordinate systems and basic geometric concepts
- **Trigonometry**: Sine, cosine functions and angle measurements
- **Programming**: Basic Python syntax and NumPy familiarity

### Mathematical Notation

Standard mathematical notation is used throughout:

- **Vectors**: Bold lowercase (𝐯, 𝐮) or arrow notation
- **Matrices**: Bold uppercase (𝐀, 𝐁) or bracket notation
- **Scalars**: Regular italic (a, b, c)
- **Operations**: Standard symbols (·, ×, ⊗)

## Usage Instructions

1. **Setup Environment**: Ensure NumPy and matplotlib are installed
2. **Sequential Learning**: Follow notebooks in numerical order
3. **Interactive Exploration**: Modify examples to test understanding
4. **Mathematical Verification**: Check results using multiple methods
5. **Geometric Visualization**: Study plots to build intuitive understanding

This comprehensive linear algebra foundation prepares students for advanced machine learning techniques including dimensionality reduction, optimization methods, and machine learning algorithms that rely heavily on linear algebraic concepts.
