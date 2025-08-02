## Overview of Q2F-Phys
Q2F-Phys: A Label-Quantized Coarse-to-Fine Framework for Robust and Efficient Physiological Measurement
<p align="center">
  <img src="assets/figures/Overview.png" alt="Framework Overview" width="800"/>
</p>

## ⚙️ Setup
```bash
bash setup.sh
```

## 🖥️ Testing with Pre-trained Models
Please refer to the configuration files located in `./configs/infer_configs`.

### Intra-Dataset Evaluation (Example)
To run the pre-trained model for **intra-dataset** evaluation (i.e., training and testing on the same dataset), you can use the following example:
- **MMPD → MMPD**:
```bash
python main.py --config_file ./configs/infer_configs/MMPD_MMPD_Q2FPhys.yaml
```

### Cross-Dataset Evaluation (Examples)
To run the pre-trained model for **cross-dataset** evaluation (i.e., training and testing on different datasets), you can refer to the following examples:

- **PURE → UBFC**:
```bash
python main.py --config_file ./configs/infer_configs/PURE_UBFC_Q2FPhys.yaml
```

- **UBFC → PURE**:
```bash
python main.py --config_file ./configs/infer_configs/UBFC_PURE_Q2FPhys.yaml
```


## 🧮 Computing Model Complexity
To calculate the model's number of parameters, MACs (multiply–accumulate operations), and throughput:
```
python model_Para_MACs_Thro.py
```


## 🎓 Acknowledgement
This work builds upon the [rPPG-Toolbox](https://github.com/ubicomplab/rPPG-Toolbox) [1].  
We sincerely thank the authors for providing this valuable resource to the community.



## References
[1] Liu, Xin, et al. "rppg-toolbox: Deep remote ppg toolbox." *Advances in Neural Information Processing Systems*, vol. 36, 2024.
