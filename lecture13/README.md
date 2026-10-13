# Lecture #13 (Association Rule Mining and Pattern Discovery)

This folder contains the supporting material used during Lecture #13 of the Data Mining and Machine Learning KSD course (Autumn 2026) **on 26 November 2026**.

## Overview

This lecture covers comprehensive association rule mining techniques essential for discovering interesting relationships and patterns in transactional datasets. All examples are provided as interactive Jupyter Notebooks with detailed explanations, code implementations, and visualizations using real-world retail data.

## Content Structure

### Core Association Rule Mining Notebooks

#### 1. **Apriori Algorithm** (`ex01_ipriori_algorithm.ipynb`)

- **Learning Objectives**: Understanding the Apriori algorithm for mining frequent itemsets and generating association rules
- **Techniques Covered**:
  - Frequent itemset mining with minimum support threshold
  - Association rule generation
  - Support, confidence, and lift metrics
  - Rule filtering and selection strategies
  - Transaction data encoding
- **Key Tools**: mlxtend frequent_patterns (apriori, association_rules), pandas, matplotlib, seaborn
- **Practical Applications**: Market basket analysis, product recommendation systems, cross-selling strategies

**Key Features**:

- Custom table rendering for frequent itemsets visualization
- Data preprocessing and cleaning for retail transactions
- Shopping cart creation from transactional data
- Association rule evaluation with lift and confidence thresholds
- Scatter plot visualization of rule metrics

#### 2. **FP-Growth Algorithm** (`ex02_fp_growth_algorithm.ipynb`)

- **Learning Objectives**: Understanding the FP-Growth algorithm as an efficient alternative to Apriori
- **Techniques Covered**:
  - FP-Tree construction for frequent pattern mining
  - Efficient frequent itemset discovery without candidate generation
  - Association rule generation from FP-Growth results
  - Comparative analysis with Apriori algorithm
  - Interactive data visualization with TreeMaps
- **Key Tools**: mlxtend fpgrowth, Plotly Express, pandas, matplotlib
- **Practical Applications**: Large-scale retail analytics, inventory management, customer behavior analysis

**Key Features**:

- Efficient mining of frequent itemsets using FP-Growth
- Custom table rendering for results display
- Interactive TreeMap visualization of top products
- Real-world retail dataset analysis (Online Retail dataset)
- Performance comparison considerations with Apriori

## Educational Features

All notebooks include:

- 📚 **Clear Learning Objectives** for each topic
- 🔍 **Step-by-step Explanations** with theoretical background
- 💻 **Hands-on Code Examples** with detailed comments
- 📊 **Interactive Visualizations** using matplotlib, seaborn, and Plotly
- 📈 **Statistical Analysis** of association rules
- 🎯 **Real-world Applications** using retail transaction data
- ✅ **Best Practices** for rule mining and evaluation
- ⚠️ **Common Pitfalls** and how to avoid them
- 🎨 **Professional Visualizations** with custom color schemes
- 📝 **Comprehensive Summaries** with key takeaways

## Technical Requirements

- **Python 3.x** with data science libraries
- **Core Libraries**: pandas, NumPy, matplotlib, seaborn
- **Association Rule Mining**: mlxtend (frequent_patterns module)
- **Interactive Visualization**: Plotly Express
- **Data Processing**: openpyxl (for Excel file handling)
- **Development Environment**: Jupyter Notebook or VS Code with notebook support
- **Dataset**: Online Retail dataset (included in `data/` folder)

## Additional Resources

### Python Scripts

Original Python scripts are also available for command-line execution:

- `ex01_ipriori_algorithm.py`
- `ex02_fp_growth_algorithm.py`

### Folders

- **`data/`**: Retail transaction dataset used in the notebooks (DVC managed)

### Files

- **`data.dvc`**: Data Version Control file for dataset management

## Dataset Information

The notebooks use the **Online Retail Dataset**, which contains:

- Transactional data from an online retail store
- Multiple attributes including InvoiceNo, Description, Quantity, Country
- Real-world shopping cart information
- Focus on transactions from specific countries (e.g., Portugal)

## Learning Path

**Recommended sequence for maximum learning effectiveness:**

1. **Apriori Foundation** (Ex 1): Start with the classic algorithm

   - Understand frequent itemset mining fundamentals
   - Learn support, confidence, and lift metrics
   - Practice rule evaluation and filtering

2. **FP-Growth Efficiency** (Ex 2): Explore the optimized approach
   - Compare with Apriori methodology
   - Understand FP-Tree construction
   - Learn advanced visualization techniques

Each notebook builds upon fundamental concepts of association rule mining, providing both theoretical understanding and practical implementation skills for real-world market basket analysis.

## Usage Instructions

1. **Setup Environment**: Ensure all required Python libraries are installed

   ```bash
   pip install pandas numpy matplotlib seaborn mlxtend plotly openpyxl
   ```

2. **Data Access**: Ensure the Online Retail dataset is available in `data/` folder

3. **Launch Notebooks**: Open notebooks in Jupyter or VS Code

4. **Follow Sequence**: Work through notebooks in the recommended order

5. **Run Python Scripts**: Alternatively, execute `.py` files directly from terminal

   ```bash
   python lecture13/ex01_ipriori_algorithm.py
   python lecture13/ex02_fp_growth_algorithm.py
   ```

6. **Experiment**: Modify parameters (min_support, min_threshold) and test with different countries

## Key Concepts Covered

- **Frequent Itemset Mining**: Discovering sets of items that frequently appear together
- **Support**: Proportion of transactions containing an itemset
- **Confidence**: Conditional probability of consequent given antecedent
- **Lift**: Ratio of observed support to expected support (independence measure)
- **Apriori Principle**: If an itemset is infrequent, all its supersets are infrequent
- **FP-Tree**: Compact data structure for efficient pattern mining
- **Market Basket Analysis**: Discovering purchasing patterns in retail data
- **Rule Evaluation**: Filtering and ranking association rules by interestingness measures

## Practical Applications

- **Retail**: Product placement, promotional bundles, cross-selling strategies
- **E-commerce**: Recommendation systems, "customers who bought X also bought Y"
- **Inventory Management**: Stock optimization based on purchasing patterns
- **Marketing**: Targeted campaigns based on product associations
- **Healthcare**: Treatment pattern analysis, drug interaction studies
- **Web Analytics**: Page visit patterns, clickstream analysis

This comprehensive collection provides both theoretical understanding and practical skills for effective association rule mining in real-world data mining and machine learning applications, from traditional Apriori to efficient FP-Growth algorithms.
