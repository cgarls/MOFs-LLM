# MOFs-LLM: Corpus Data Processing and Fine-Tuning Analysis

## Overview
MOFs-LLM is a domain-customized large language model (LLM) tailored for metal-organic frameworks (MOFs) through post-training. This repository contains the code for corpus data processing and supervised fine-tuning result analysis, supporting the development of high-performance hydrogen storage materials.

## Features
- **Corpus Processing**: Handles a large-scale dataset (>210 million tokens) with detailed descriptions of 15,000 MOF structures.
- **Fine-Tuning Analysis**: Evaluates the model’s ability to predict hydrogen storage performance and design synthesizable MOFs.
- **MOFs-LLM Model**: Leverages ERNIE post-training to capture complex structure-property relationships.

## Repository Structure
```
├── data/                 # Corpus dataset and preprocessing scripts
├── notebooks/            # Jupyter notebooks for data analysis and visualization
├── Pictures/              # Performance metrics and analysis outputs
├── README.md             # Project documentation
```

Workflow and Summary
Below are the flow chart and graphic summary of the MOFs-LLM project:

![Graphic summary](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Graphic%20summary.png)
![Flow chart](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Flow%20chart.png)

## Installation
### Prerequisites
- Python 3.8+
- PyTorch
- Hugging Face Transformers
- pandas, numpy, and other dependencies

```bash
pip install -r requirements.txt
```

## Results
MOFs-LLM achieved a **94.8% prediction accuracy** for hydrogen storage properties and successfully assisted in the synthesis of a top-performing MOF material (1.3 wt% storage at room temperature).

## Citation
If you use this code, please cite our work:
```
@article{mofs-llm,
  author    = {Your Name et al.},
  title     = {MOFs-LLM: A Large Language Model for Metal-Organic Frameworks},
  journal   = {ArXiv},
  year      = {2025},
}
```

## License
This project is licensed under the MIT License.
