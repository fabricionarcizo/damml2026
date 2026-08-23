# Data Mining and Machine Learning KSD (2026)

This course introduces data mining and machine learning with a strong emphasis on practical and applied problem-solving. Students will explore fundamental concepts and techniques for both pattern discovery and predictive modeling, including classification, regression, clustering, dimensionality reduction, association rule mining, and data preprocessing. The course focuses on analyzing real-world data problems, selecting appropriate methods, and developing end-to-end data science workflows, from data preparation and feature engineering to model training, evaluation, and communication of results. Through hands-on exercises, students will work with modern software libraries and real-world datasets, combining established tools with the implementation of core algorithms.

## Setup the Development Environment

This repository contains the configuration files to set up the development environment. It uses `conda` to manage a Python development environment and all required packages and libraries this project uses. We use [Data Version Control (DVC)](http://dvc.org) to store all binary files (videos, images, timesheets, among others) used by examples and exercises of this course. These files are available in a private bucket on [Amazon S3](https://aws.amazon.com/s3), and the students can access them as read-only resources via an HTTPS connection. The following presents the step-by-step tutorial on setting up the `damml2026` development environment.

### Requirements

- An active [Anaconda](https://anaconda.org), [Miniconda](https://docs.anaconda.com/miniconda/miniconda-install), or [Miniforge](https://github.com/conda-forge/miniforge) (highly recommended) installation with the `bin` folder added to the *Environmental Variable* `$PATH` (Linux and macOS) or `%PATH%` (Microsoft Windows).
- An integrated development environment with C/C++ compiler and libraries, such as [Xcode](https://developer.apple.com/xcode) for macOS users, [GCC](https://gcc.gnu.org) for Linux users, and [Visual Studio 2022](https://visualstudio.microsoft.com) for Microsoft Windows users.
- [CMake](https://cmake.org), a cross-platform, open-source build system generator.
- (Recommended) [Visual Studio Code](https://code.visualstudio.com) installed.

### Installation

First of all, use the Terminal (**Prompt**) to execute the following commands. Clone this repository and enter the project root folder:

```[bash]
git clone https://github.com/fabricionarcizo/damml2026
cd $PROJECT\damml2026
```

Then, create a new environment called `damml2026`:

```[bash]
conda env create --file=./environment.yml
```

Activate the created environment:

```[bash]
conda activate damml2026
```

Install the required Python packages and libraries:

```[bash]
poetry install --no-root
```

Finally, download the binary resource available in our private Amazon S3 bucket:

```[bash]
dvc pull
```

**IMPORTANT**: Before each lecture, you must download the newest binary files by executing the command `dvc pull` again.

**P.S.**: Once in a while, update your development environment to get the latest pip package versions:

```[bash]
git pull
conda env update --file=./environment.yml --prune
poetry install --no-root
```

## Description

Data mining and machine learning have become essential for extracting knowledge and building intelligent systems from data, due to the rapid growth in data availability and computational capabilities. Modern applications across domains such as healthcare, finance, and digital platforms rely on data-driven models to support decision-making, automate processes, and generate insights. However, developing such solutions involves several challenges, including handling large and complex datasets, selecting appropriate algorithms, ensuring model generalization, and evaluating performance in real-world scenarios. This course provides fundamental and practical knowledge for analyzing data and developing machine learning models using modern tools and methodologies, emphasizing hands-on experience and real-world problem-solving. The course introduces the following topics:

- The data mining and machine learning process.
- Data preprocessing, feature engineering, and exploratory data analysis.
- Supervised learning techniques, including classification and regression.
- Unsupervised learning techniques, including clustering and dimensionality reduction.
- Pattern and association rule mining.
- Model evaluation, validation strategies, and performance metrics.
- Advanced topics such as neural networks, deep learning, and anomaly detection.

The course emphasizes practical, hands-on learning using real-world datasets and modern software libraries. Students will develop end-to-end data analysis workflows, from data preparation to model evaluation and result communication. Application examples will be drawn from domains such as demographics, image processing, multimodal interaction, and healthcare.

### Use of generative AI during the exam: 

The use of generative artificial intelligence is permitted during the exam, provided that students comply with the official ITU guidelines on generative AI.

## Formal Prerequisites

Students are expected to have prior programming experience and be comfortable implementing algorithms independently from high-level descriptions. This corresponds to having completed at least an introductory programming course, preferably at an intermediate level. The course includes compulsory programming in [Python](http://python.org).

Students should also be familiar with basic mathematical concepts and notation, including variables, functions, sets, and fundamental statistics (e.g., mean and variance). Basic knowledge of linear algebra (e.g., vectors and matrices) is beneficial.

### Information about study structure

This is a specialization course within the [MSc Software Design](https://en.itu.dk/Programmes/MSc-Programmes/Software-Design) study programme and an elective for other MSc programmes. Students must meet the general admission requirements of the [IT University of Copenhagen](https://en.itu.dk).

## Intended Learning Outcomes

After the course, the student should be able to:

- Explain the fundamental concepts of data mining and machine learning, including supervised and unsupervised learning approaches, and identify their typical application contexts.
- Analyze real-world data problems and select appropriate data mining and machine learning methods based on data characteristics, problem constraints, and desired outcomes.
- Implement key algorithms for data preprocessing (e.g., normalization, handling missing data, dimensionality reduction), association rule mining, classification, clustering, and basic machine learning models.
- Train, evaluate, and compare machine learning models using appropriate validation strategies and performance metrics (e.g., accuracy, precision, recall, F1 score, ROC/AUC).
- Design, execute, and reflect on end-to-end data analysis workflows, including data preparation, feature engineering, model training, evaluation, and result communication, using modern software libraries such as Pandas, Matplotlib, Plotly, Seaborn, Scikit-Learn, PyTorch, TensorFlow, and Keras.
- Collaborate effectively in project teams to address data-driven problems, document findings, interpret the results critically, and present conclusions clearly to both technical and non-technical audiences.

## Learning Activities

The course spans 14 weeks, with two-hour lectures and two-hour exercise sessions per week.

Lectures introduce the theoretical foundations of data mining and machine learning, supported by practical examples and demonstrations of key algorithms and techniques. Exercise sessions focus on hands-on learning, in which students independently implement algorithms and work with real-world datasets in Python.

The course includes a mandatory midterm assignment, in which students apply the techniques and methods covered in the first part of the course to solve a data-driven problem.

In the final part of the course, students will complete a group-based project (2–4 students) in which they define and develop a data mining and machine learning solution for a relevant real-world problem. This project emphasizes the design and execution of end-to-end data analysis workflows, including data preprocessing, feature engineering, model training, evaluation, and communication of results.

In addition to lectures and exercise sessions, supervision meetings are provided to support the group projects. These sessions complement the theoretical material and guide students in applying concepts to practical scenarios. Overall, the course emphasizes a balance between theoretical understanding and practical implementation, requiring active participation and programming throughout.

The following table presents the lecture plan:

| Week | Date       | Lecture                                                  |
| ---- | ---------- | -------------------------------------------------------- |
| 01   | 27/08/2026 | [Getting Started](lecture01)                             |
| 02   | 03/09/2026 | [Introduction to Machine Learning](lecture02) |
| 03   | 10/09/2026 | [Mathematical Foundations for Machine Learning](lecture03)              |
| 04   | 17/09/2026 | [Data Preprocessing and Feature Engineering](lecture04)                          |
| 05   | 24/09/2026 | [Exploratory Data Analysis and Visualization](lecture05)          |
| 06   | 01/10/2026 | [Regression](lecture06)              |
| 07   | 08/10/2026 | [Classification: Foundations](lecture07)         |
| 08   | 22/10/2026 | [Classification: Advanced Models](lecture08)                         |
| 09   | 29/10/2026 | [Model Evaluation and Selection](lecture09)                  |
| 10   | 05/11/2026 | [Clustering](lecture10)             |
| 11   | 12/11/2026 | [Dimensionality Reduction and Representation](lecture11)                    |
| 12   | 19/11/2026 | [Anomaly and Outlier Detection](lecture12)                           |
| 13   | 26/11/2026 | [Association Rule Mining and Pattern Discovery](lecture13)                     |
| 14   | 03/12/2026 | [Final Exam Project and Course Evaluation](lecture14)    |

## Mandatory Activities

Students must complete one mandatory assignment in which they apply data mining and machine learning techniques to a given dataset. The assignment involves implementing selected methods, performing data preprocessing, training and evaluating models, and presenting the results in a written report.

The assignment is assessed on a pass/fail basis (**"Approved"**/**"Not Approved"**) and is accompanied by feedback to support student learning.

The pedagogical purpose of the mandatory assignment is to provide hands-on experience aligned with the course learning objectives, including data preparation, model development, and evaluation in a practical context.

Students who submit but do not pass the mandatory assignment must resubmit it by a specified deadline, typically within one month of receiving the grade.

The student will receive the grade **NA** (**not approved**) at the ordinary exam, if the mandatory activities are not approved and the student will use an exam attempt.

## Course Literature

**The 100-Page Machine Learning Book**. By Andriy Burkov. Published Jan 13, 2019 by Lightning Source Inc. ISBN-10 1777005477 and ISBN-13 978-1777005474.

**Data Mining: Concepts and Techniques (The Morgan Kaufmann Series in Data Management Systems), 4th Edition**. By Jiawei Han, Micheline Kamber, and Jian Pei. Published Oct 17, 2022 by Morgan Kaufmann. ISBN-10 9780128117606 and ISBN-13 978-0128117606.

## Student Activity Budget

Estimated distribution of learning activities for the typical student:

- Preparation for lectures and exercises: 20%
- Lectures: 15%
- Exercises: 10%
- Assignments: 10%
- Project work, supervision included: 35%
- Exam with preparation: 10%

## Ordinary Exam

### Exam type

D: Submission of written work with following oral, External (7-point scale)

### Exam variation

D1G: Submission for groups with following oral exam based on the submission. Shared responsibility for the report.

### Exam submission description

The final assessment will be a jointly written report. There will be a group presentation of this report followed by individual questions about the report and the work behind it, resulting in individual grades.

### Group submission

#### Group

2-4

### Exam duration per student for the oral exam

20 minutes

### Group exam form

Mixed exam 2: Joint student presentation followed by an individual dialogue. The group makes their presentations together and afterwards the students participate in the dialogue individually while the rest of the group is outside the room.

## Reexam

### Reexam type

B: Oral exam

### Reexam variation

B22: Oral exam with no time for preparation.

### Reexam duration per student for the oral exam

20 minutes

## Time and Date

Ordinary Exam - submission Mon, 04 Jan 2027, 08:00 - 14:00

Ordinary Exam Mon, 18 Jan 2027, 09:00 - 21:00

Ordinary Exam Tue, 19 Jan 2027, 09:00 - 21:00

Ordinary Exam Wed, 20 Jan 2027, 09:00 - 21:00
