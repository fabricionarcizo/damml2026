# Lecture #01: Getting Started

This folder contains the supporting materials used during **Lecture #01** of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 27 August 2026**.

## Overview

This lecture introduces fundamental Python programming concepts essential for data mining and machine learning. The materials progress from basic Python syntax to advanced data manipulation using popular libraries like pandas and NumPy. All examples are provided as interactive materials combining theoretical explanations with hands-on coding practice.

Python serves as the primary programming language for modern data science and mining applications, offering powerful libraries, clear syntax, and extensive community support for analytical tasks.

## Learning Objectives

By the end of this lecture, students will be able to:

- Master Python syntax and fundamental programming constructs
- Work proficiently with core data types (strings, numbers, lists, tuples, dictionaries)
- Implement control flow structures (conditionals, loops) for algorithmic thinking
- Create and utilize functions for code organization and reusability
- Perform comprehensive data manipulation with pandas DataFrame operations
- Load, explore, and analyze CSV data files systematically
- Calculate and interpret basic statistical measures for data understanding
- Apply Python programming skills to real-world data mining and machine learning scenarios

## Content Structure

### Python Fundamentals

#### 1. **First Python Program** (`ex01_first_python_program.py`)

- **Learning Objectives**: Introduction to Python program structure and execution
- **Concepts Covered**:
  - Basic Python syntax and program structure
  - Print statements and output formatting
  - Comments and documentation practices
  - Python interpreter and execution model
- **Key Tools**: Python interpreter, basic I/O operations
- **Applications**: Program structure understanding, debugging basics, development workflow

#### 2. **Jupyter Notebook Introduction** (`ex02_first_jupyter_notebook.ipynb`)

- **Learning Objectives**: Mastering interactive development with Jupyter notebooks
- **Concepts Covered**:
  - Jupyter notebook interface and functionality
  - Code cells vs. markdown cells
  - Kernel management and execution
  - Notebook best practices and organization
- **Key Tools**: Jupyter notebook interface, markdown formatting, code execution
- **Applications**: Interactive data analysis, documentation, reproducible research

#### 3. **Python Syntax Fundamentals** (`ex03_basic_python_syntax.ipynb`)

- **Learning Objectives**: Understanding Python's syntactic rules and conventions
- **Concepts Covered**:
  - Indentation and code structure
  - Comments and docstrings
  - Basic syntax rules and conventions
  - Error types and debugging basics
- **Key Tools**: Python syntax checker, error interpretation, code formatting
- **Applications**: Clean code writing, debugging skills, professional development practices

### Data Types and Variables

#### 4. **Variables and Assignment** (`ex04_variables_and_assignment.ipynb`)

- **Learning Objectives**: Mastering variable concepts and data type fundamentals
- **Concepts Covered**:
  - Variable assignment and naming conventions
  - Dynamic typing and type inference
  - Basic data types (int, float, bool, str)
  - Memory management and variable scope
- **Key Tools**: Type checking functions, variable inspection, memory analysis
- **Applications**: Data storage, type management, efficient programming practices

#### 5. **String Operations** (`ex05_basic_strings_operations.ipynb`)

- **Learning Objectives**: Comprehensive string manipulation and text processing
- **Concepts Covered**:
  - String creation and formatting techniques
  - String methods and operations
  - Text processing and pattern matching
  - Unicode and encoding considerations
- **Key Tools**: String methods, formatting operations, regular expressions basics
- **Applications**: Text data cleaning, data parsing, report generation

### Input/Output Operations

#### 6. **Simple Input/Output** (`ex06_simple_input_output.ipynb`)

- **Learning Objectives**: Managing basic console-based data exchange
- **Concepts Covered**:
  - Input() function and user interaction
  - Output formatting and print options
  - Type conversion for input processing
  - Error handling for user input
- **Key Tools**: Console I/O functions, type conversion, input validation
- **Applications**: User interfaces, data collection, interactive programs

#### 7. **Enhanced Input/Output** (`ex07_enhanced_input_output.ipynb`)

- **Learning Objectives**: Creating user-friendly graphical input interfaces
- **Concepts Covered**:
  - EasyGUI library for dialog boxes
  - File selection and directory navigation
  - Message boxes and user notifications
  - Enhanced user experience design
- **Key Tools**: EasyGUI library, file dialogs, user interface design
- **Applications**: User-friendly data collection, file processing, interactive analytics

### Control Flow Structures

#### 8. **Conditional Statements** (`ex08_conditional_statements.ipynb`)

- **Learning Objectives**: Implementing decision-making logic and branching
- **Concepts Covered**:
  - If, elif, else statement structures
  - Boolean logic and comparison operators
  - Nested conditionals and complex logic
  - Ternary operators and concise expressions
- **Key Tools**: Logical operators, comparison functions, boolean algebra
- **Applications**: Data filtering, decision trees, algorithmic logic

#### 9. **For Loops** (`ex09_for_loops.ipynb`)

- **Learning Objectives**: Mastering iterative processing with definite loops
- **Concepts Covered**:
  - For loop syntax and iteration patterns
  - Range function and sequence generation
  - Nested loops and complex iterations
  - List comprehensions and iterator protocols
- **Key Tools**: Range functions, iterators, comprehension syntax
- **Applications**: Data processing, batch operations, algorithmic implementations

#### 10. **While Loops** (`ex10_while_loops.ipynb`)

- **Learning Objectives**: Implementing conditional iteration and indefinite loops
- **Concepts Covered**:
  - While loop syntax and condition checking
  - Loop control statements (break, continue)
  - Infinite loops and termination conditions
  - Loop optimization and efficiency
- **Key Tools**: Conditional expressions, loop controls, termination logic
- **Applications**: Data streaming, condition-based processing, algorithmic solutions

### Functions and Modular Programming

#### 11. **Simple Functions** (`ex11_using_simple_functions.ipynb`)

- **Learning Objectives**: Creating reusable code blocks and modular programming
- **Concepts Covered**:
  - Function definition and calling syntax
  - Parameters and arguments (positional, keyword)
  - Return statements and value passing
  - Local vs. global scope management
- **Key Tools**: Function definition syntax, parameter handling, scope analysis
- **Applications**: Code reusability, modular design, algorithmic abstraction

### Data Structures

#### 12. **List Operations** (`ex12_basic_list_operations.ipynb`)

- **Learning Objectives**: Mastering dynamic arrays and sequence manipulation
- **Concepts Covered**:
  - List creation, indexing, and slicing
  - List methods and operations (append, extend, remove)
  - List comprehensions and functional operations
  - Nested lists and multidimensional data
- **Key Tools**: List methods, slicing operations, comprehensions
- **Applications**: Data collection, sequence processing, data structure implementation

#### 13. **Tuple Operations** (`ex13_basic_tuple_operations.ipynb`)

- **Learning Objectives**: Understanding immutable sequences and data integrity
- **Concepts Covered**:
  - Tuple creation and immutability properties
  - Tuple unpacking and multiple assignment
  - Named tuples and structured data
  - Performance considerations and use cases
- **Key Tools**: Tuple operations, unpacking syntax, named tuple factory
- **Applications**: Immutable data storage, coordinate systems, return multiple values

#### 14. **Dictionary Operations** (`ex14_basic_dictionary_operations.ipynb`)

- **Learning Objectives**: Implementing key-value mappings and associative arrays
- **Concepts Covered**:
  - Dictionary creation and key-value relationships
  - Dictionary methods and operations
  - Dictionary comprehensions and transformations
  - Hash tables and performance characteristics
- **Key Tools**: Dictionary methods, key access patterns, comprehension syntax
- **Applications**: Data mapping, lookup tables, configuration management

### Data Analysis with Pandas

#### 15. **CSV File Loading** (`ex15_load_csv_file.ipynb`)

- **Learning Objectives**: Importing and exploring structured data files
- **Concepts Covered**:
  - Pandas library introduction and DataFrame concept
  - CSV reading with various options and parameters
  - Data type inference and conversion
  - Initial data exploration and inspection methods
- **Key Tools**: pandas.read_csv(), DataFrame methods, data inspection functions
- **Applications**: Data import, file processing, initial data assessment

#### 16. **Data Manipulation** (`ex16_simple_data_manipulation.ipynb`)

- **Learning Objectives**: Performing essential data filtering and selection operations
- **Concepts Covered**:
  - DataFrame indexing and selection methods
  - Boolean indexing and conditional filtering
  - Column operations and transformations
  - Data cleaning and preparation techniques
- **Key Tools**: DataFrame selection methods, boolean indexing, column operations
- **Applications**: Data filtering, subset analysis, data preparation pipelines

#### 17. **Basic Statistics** (`ex17_basic_statistics.ipynb`)

- **Learning Objectives**: Computing and interpreting fundamental statistical measures
- **Concepts Covered**:
  - Descriptive statistics (mean, median, mode, standard deviation)
  - Distribution analysis and data exploration
  - Correlation and relationship analysis
  - Statistical summary and reporting methods
- **Key Tools**: pandas statistical methods, NumPy functions, statistical analysis
- **Applications**: Data summarization, exploratory analysis, statistical reporting

## Educational Features

All materials include:

- 🐍 **Progressive Learning** from basic syntax to data analysis
- 💡 **Interactive Examples** with immediate feedback and execution
- 📚 **Comprehensive Explanations** linking theory to practical application
- 🔧 **Hands-on Exercises** reinforcing each concept through practice
- 📊 **Real Data Examples** using authentic datasets for analysis
- 🎯 **Practical Applications** connecting concepts to data mining and machine learning workflows
- ✅ **Best Practices** for writing clean, efficient Python code
- ⚠️ **Common Mistakes** and debugging techniques
- 📝 **Code Documentation** and professional development practices

## Technical Requirements

- **Python 3.12+** with core libraries and data science packages
- **Core Libraries**: pandas, NumPy, EasyGUI for enhanced functionality
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Data Files**: Sample CSV datasets included in `data/` folder (managed with DVC)

## Additional Resources

### Folders

- **`data/`**: Sample datasets used for data analysis exercises (DVC managed)
- **`exercises/`**: Additional practice exercises and supplementary datasets

### Files

- **`data.dvc`**: Data Version Control file for dataset management
- **`.gitignore`**: Git configuration for version control
- **`ex01_first_python_program.py`**: Stand-alone Python script for basic program structure

## Learning Path

**Recommended sequence for building Python proficiency:**

### Foundation Level (Ex 1-7): Python Basics

- Program structure → Jupyter introduction → Syntax fundamentals → Variables and I/O

### Intermediate Level (Ex 8-11): Control Structures

- Conditionals → Loop constructs → Function creation and modular programming

### Advanced Level (Ex 12-17): Data Structures and Analysis

- Built-in data types → pandas introduction → Data manipulation → Statistical analysis

Each section builds essential programming skills needed for advanced data mining and machine learning techniques and algorithmic implementation.

## Prerequisites and Setup

### Required Software Installation

```bash
# Using pip (recommended)
pip install pandas numpy easygui jupyter

# Using conda (alternative)
conda install pandas numpy jupyter
pip install easygui
```

### Environment Verification

```python
# Test imports in Python/Jupyter
import pandas as pd
import numpy as np
import easygui as eg
print("All libraries imported successfully!")
```

## Assessment and Practice

### Learning Activities

Each notebook includes:

- **Conceptual Explanations** with clear examples and use cases
- **Interactive Code Cells** for immediate practice and experimentation
- **Progressive Exercises** building from simple to complex applications
- **Real-world Applications** connecting concepts to data mining and machine learing scenarios
- **Debugging Practice** with common errors and solutions
- **Best Practices** for writing maintainable and efficient code

### Skill Development Focus

- **Syntactic Proficiency**: Writing clean, readable Python code
- **Problem Decomposition**: Breaking complex tasks into manageable steps
- **Data Handling**: Working effectively with different data types and structures
- **Analytical Thinking**: Using programming constructs for data analysis
- **Documentation**: Creating clear, well-commented code

## Usage Instructions

1. **Environment Setup**: Install Python, Jupyter, and required libraries
2. **Repository Access**: Clone or download course materials
3. **Sequential Learning**: Follow notebooks in numerical order for optimal progression
4. **Active Practice**: Modify examples and create variations to test understanding
5. **Data Exploration**: Use provided datasets to practice new concepts

## Connection to Data Mining and Machine Learning

This Python foundation directly supports advanced data mining and machine learning concepts:

- **Data Preprocessing**: Using pandas for cleaning and transformation
- **Algorithm Implementation**: Programming machine learning algorithms from scratch
- **Statistical Analysis**: Computing measures and testing hypotheses
- **Visualization**: Creating plots and charts for data exploration
- **Automation**: Building data processing pipelines and workflows

## Next Steps

Upon completion, students will be prepared for:

- **Lecture #03**: Mathematical foundations for data mining and machine learing algorithms
- **Advanced Python**: Object-oriented programming and advanced pandas operations
- **Data Mining Algorithms**: Implementation of clustering, classification, and regression
- **Machine Learning**: Scikit-learn library and model development workflows

This comprehensive Python introduction ensures students have the programming foundation necessary for successful participation in advanced data mining and machine learning coursework and practical applications.
