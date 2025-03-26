# MOFs-LLM: Bridging Virtual to Real through Inverse Design of MOFs for Hydrogen Storage

## 🌟 Breakthrough Research
**Domain-customized LLM for MOFs** achieving:
- 94.8% accuracy in hydrogen storage prediction
- Successful synthesis of Cu-LLMs-1 (1.33 wt% capacity at RT)

## 📌 Core Innovation
We present **MOFs-LLM**, the first vertical LLM for metal-organic frameworks that:
1. **Understands** complex MOF characteristics across electronic/atomic/structural hierarchies
2. **Predicts** hydrogen storage performance with 94.8% accuracy
3. **Designs** synthesizable MOF structures through reverse design
4. **Guides** experimental synthesis with actionable recommendations

## 🧠 Technical Foundation
### Domain-Specific Pretraining
- **Corpus**: 210M+ tokens covering 15,000 MOF structures
- **Knowledge Integration**: 
  - 6,000+ research papers 
  - Experimental synthesis protocols
  - Structure-property relationships
- **Model Architecture**: ERNIE-based post-training

##Workflow and Summary
###Below are the flow chart and graphic summary of the MOFs-LLM project:

![Graphic summary](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Graphic%20summary.png)
![Flow chart](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Flow%20chart.png)

## Results
MOFs-LLM achieved a **94.8% prediction accuracy** for hydrogen storage properties and successfully assisted in the synthesis of a top-performing MOF material (1.3 wt% storage at room temperature).

## Citation
If you use this code, please cite our work:
```
@article{mofsllm,
  title={Bridging Virtual to Real: Inverse Design of MOFs for Hydrogen Storage},
  author={Liu, Zhimeng and Su, Yuqiao and Gao, Hongyi and Shi, Lei and Wang, Ge},
  journal={Nature Materials},
  year={xxxx},
  doi={xxxx}
}
```

## License
This project is licensed under the MIT License.


# MOFs-LLM: Bridging Virtual Design to Experimental Reality for Hydrogen Storage

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Overview
This repository presents MOFs-LLM, the first domain-specific large language model for inverse design of metal-organic frameworks (MOFs) with both high hydrogen storage capacity and experimental synthesizability. Our work addresses two critical challenges in MOF research:
1. Bridging the gap between hypothetical structures and experimentally viable materials
2. Simultaneously optimizing hydrogen storage performance and synthetic feasibility

## Key Innovations
- ​**Domain-Specialized LLM**: 210M-token MOF corpus integrating structural descriptions, synthesis protocols, and performance data
- ​**Dual Optimization**: Achieves 94.8% prediction accuracy for hydrogen storage while maintaining synthesizability
- ​**Experimental Validation**: Successfully synthesized Cu-LLMs-1 with 1.33 wt% room-temperature hydrogen adsorption (top 5 among pure MOFs)

## Methodology
### Training Pipeline
![Training Flowchart](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Flow%20chart.png)

1. ​**Post-Pretraining**:
   - Domain adaptation of ERNIE model using comprehensive MOF corpus
   - Captures hierarchical structural features (metal centers, ligands, topologies)

2. ​**Supervised Fine-Tuning**:
   - Multi-task learning for hydrogen capacity prediction and synthesis feasibility
   - Incorporates expert knowledge from 6,000+ research papers

3. ​**Inverse Design**:
   - Conditional generation of novel MOF structures
   - Experimental feedback loop for synthesis optimization

## From Virtual to Reality
![Research Breakthrough](https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Graphic%20summary.png)

Our framework demonstrates:
- ​**3 experimental iterations** to identify optimal synthesis conditions
- ​**1.33 wt% hydrogen capacity** at room temperature
- ​**Top 5 performance** among pure MOF materials

## Getting Started
### Prerequisites
- Python 3.8+
- PyTorch 1.12+
- Transformers library

### Basic Usage
```python
from mofs_llm import MOFsLLMPipeline

# Load pretrained model
designer = MOFsLLMPipeline.from_pretrained("MOFs-LLM-base")

# Generate MOF candidates
target_properties = {"H2_capacity": ">1.2wt%", "temperature": "298K"}
candidates = designer.inverse_design(target_properties)
