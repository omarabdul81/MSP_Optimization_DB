# Mathematical Optimization and Databases: Solving a Multi-Site Production Planning Problem with Python

## Overview

Production planning problems are a class of optimization problems that play a vital role in various industrial and manufacturing domains. Given the scale, sparsity, and complexity of modern production networks and infrastructure, mathematical optimization based on modern optimization tools and simulation frameworks has become indispensable. These tools help manufacturers quickly and efficiently construct plans to meet strict delivery deadlines, improve productivity, eliminate underutilization/overutilization within production lines, minimize costs, and maximize profits.

Many of these mathematical optimization solutions must process large datasets residing in database systems, whether on-premises or in the cloud. The main aim of this project is to explore the development of an optimization workflow that solves a class of production planning problems by interacting with database systems. We utilize a group of open-source frameworks in Python to develop this workflow, including:

- **PuLP**: To model and solve optimization problems.
- **SQLite**: To implement the database engine.
- **pandas**: To preprocess and manipulate data.
- **matplotlib** and **seaborn**: To visualize and analyze the input and output of the optimization workflow.

The complete description of the project can be found [Here](https://link-url-here.org).

## Installation and Usage

### Clone the Repository

```bash
git clone https://github.com/your-username/project-name.git
cd project-name
```

### Install Required Packages

Follow the directions in the notebooks to install the required third-party packages.

### Setup Resource Folders

In the project home directory, set up the resource folder to store the input/output of the optimization workflows as follows:

```
├── resources
│   ├── data
│   │   ├── input
│   │   │   ├── xx.csv
│   ├── output
│   │   ├── xx.csv
│   ├── model
│   │   ├── xx.lp
```

### Start Jupyter Notebook

In the project home directory, start Jupyter Notebook:

```bash
jupyter notebook
```

### Run Notebooks

Open and run the notebooks in the following order:

1. **05_00_input_data_generator.ipynb**: Generates synthetic input data required to test optimization workflows.
2. **05_01_load_data.ipynb**: Loads input data into the SQLite3 database.
3. **05_02_multisite_optimization.ipynb**: Implements the serial optimization workflow.