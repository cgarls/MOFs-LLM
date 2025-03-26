# MOFs-LLM: Bridging Virtual to Real through Inverse Design of MOFs for Hydrogen Storage
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<img src="https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Graphic%20summary.png" width="60%" style="display: block; margin: 0 auto;" alt="MOFs-LLM research breakthrough: Bridging computational design to experimental synthesis">

## Repository Structure
```
├── data/                 # Corpus dataset and preprocessing scripts
├── notebooks/            # Jupyter notebooks for data analysis and visualization
├── Pictures/              # Performance metrics and analysis outputs
├── README.md             # Project documentation
```

## Methodology
### Training Pipeline
<img src="https://github.com/cgarls/MOFs-LLM/raw/main/Pictures/Flow%20chart.png" width="60%" style="display: block; margin: 0 auto;" alt="MOFs-LLM training workflow: Post-pretraining → Supervised Fine-Tuning → Inverse Design → Experimental Validation">

- ​**Domain-Specialized LLM**: 210M-token corpus integrating structural descriptions, MOFs papers, and materials/chemical data
- ​**Accurate Prediction**: Achieves 94.8% prediction accuracy for hydrogen storage 
- ​**Reverse Design & Experimental Validation**: Successfully synthesized Cu-LLMs-1 with 1.33 wt% room-temperature hydrogen adsorption (top 5 among pure MOFs)

## 📌 Core Innovation
We present **MOFs-LLM**, the first vertical LLM for metal-organic frameworks that:
1. **Understands** complex MOF characteristics across electronic/atomic/structural hierarchies
2. **Predicts** hydrogen storage performance with 94.8% accuracy
3. **Designs** synthesizable MOF structures through reverse design
4. **Guides** experimental synthesis with actionable recommendations

## Dataset Sources
The chemical and materials domain corpus was augmented with these high-quality datasets:

[![peS2o](https://img.shields.io/badge/Dataset-peS2o-blue)](https://huggingface.co/datasets/allenai/peS2o)  
[![ChemSum](https://img.shields.io/badge/Dataset-ChemSum-green)](https://huggingface.co/datasets/griffin/ChemSum)  

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
