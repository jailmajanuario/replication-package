# Snowballing for Review

## Overview

This repository centralizes CSV datasets exported from different snowballing and academic indexing tools, including Google Scholar, OpenAlex, Lens, Semantic Scholar, LitMaps, OpenCitations, ResearchRabbit, and SnowMap. In addition to the datasets, the repository includes analysis notebooks and auxiliary scripts used for constructing citation and reference graphs, comparing tools, and conducting analyses related to the snowballing process in systematic reviews.

Detailed instructions describing the data collection process for each tool are available in [step_tools.pdf](step_tools.pdf).

| Tool | Website |
|---|----|
| Google Scholar | https://scholar.google.com.br/ |
| OpenAlex | https://openalex.org/ |
| Lens | https://about.lens.org/ | 
| Semantic Scholar | https://www.semanticscholar.org/ |
| LitMaps | https://www.litmaps.com/ |
| OpenCitations | https://opencitations.net/ |
| ResearchRabbit | https://www.researchrabbit.ai/ |
| SnowMap | Omitted to preserve the double-blind review process. The link will be made publicly available upon paper acceptance. |

### Main Objectives

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

To install the dependencies:

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

The notebooks available in the `notebooks_analysis/` directory reproduce the analyses conducted for each research question presented in the study.

#### RQ1: *What types of article metadata can be extracted by each tool, and how complete and consistent are these data?*

```bash
jupyter notebook rq1_analysis.ipynb
```

Execute the notebook cells sequentially to reproduce the metadata extraction, comparison analyses, and visualizations.

#### RQ2: *Do the studies retrieved by the tools originate from recognized scientific sources in the Software Engineering domain?*

```bash
jupyter notebook rq2_analysis.ipynb
```

This notebook reproduces the publication venue and quartile analyses.

#### RQ3: *To what extent do the studies retrieved by each tool align with the ground truth in terms of coverage?*

```bash
jupyter notebook rq3_analysis.ipynb
```

This notebook reproduces the coverage analyses and graph-based comparisons among the evaluated tools.

#### RQ4: *To what extent can LLMs support the automated screening of studies retrieved through forward snowballing?*

Instructions for configuring and executing the LLM-related scripts are available in the README file located in the `llms_analysis/` directory.

```bash
python llms_analysis/code/analysis.py
python llms_analysis/code/compare.py
```

---


