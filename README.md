# Snowballing for Review

## Overview

This repository centralizes CSV datasets exported from different snowballing and academic indexing tools, including Google Scholar, OpenAlex, Lens, Semantic Scholar, LitMaps, OpenCitations, ResearchRabbit, and SnowMap. In addition to the datasets, the repository includes analysis notebooks and auxiliary scripts used for constructing citation and reference graphs, comparing tools, and conducting analyses related to the snowballing process in systematic reviews.

Main objectives:

- Gather and standardize metadata collected from different tools;
- Generate citation and reference graphs to support the exploration of study networks;
- Facilitate comparisons across data sources and promote the reproducibility of the analyses;
- Support the study screening process through the use of LLMs, considering inclusion and exclusion criteria defined by the researchers.

## Repository Structure

```
snowballing_for_review/
├── data/                  # Datasets exported from the tools
├── notebooks_analysis/    # Analysis and graph generation notebooks
├── llms_analysis/         # Scripts and experiments using LLMs
├── quartile/              # Data used for publication venue quartile analysis
├── step_tools.pdf         # Step-by-step process for data acquisition using the tools
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.10+ is recommended.
- All required packages are listed in `requirements.txt`.

Para instalar as dependências:

```bash
pip install -r requirements.txt
```



## How to Use

### 1. Set Up the Environment
```bash

# Clone the repository
git clone <repository-url>
cd snowballing_for_review

# Install dependencies
pip install -r requirements.txt

```
### 2. Run the Notebooks

```bash

# Jupyter Notebook
jupyter notebook

```
Open any notebook available in the `notebooks_analisys/` directory (e.g., `graph2.ipynb`) and execute the cells sequentially to reproduce the analyses, visualizations, and citation graphs presented in the study


## 3. Execute the LLM-Based Screening Scripts

Utility scripts related to the LLM-based study screening process are available in `llms_analysis/code/`.

Additional instructions for configuring and executing the LLM-related scripts are available in the README file located in the `llms_analysis/` directory.

```bash
python LLMs_Analisy/code/analysis.py
python LLMs_Analisy/code/compare.py
```



## Developed Tool: SnowMap


To preserve the double-blind review process, the link to the tool is omitted in this version of the replication package. Upon acceptance, the complete system including the frontend and backend source code will be made publicly available.

---


