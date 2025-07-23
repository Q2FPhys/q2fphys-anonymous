## Overview of Q2F-Phys
Q2F-Phys: A Label-Quantized Coarse-to-Fine Framework for Robust and Efficient Physiological Measurement
<p align="center">
  <img src="assets/figures/Overview_1.jpg" alt="Framework Overview" width="800"/>
</p>

## ⚙️ Setup
Step 1
```bash
bash setup.sh
```
Step 2
```bash
conda activate Q2FPhys
```
Step 3
```bash
pip install -r requirements.txt
```

## 🖥️ Testing with Pre-trained Models
Please refer to the configuration files located in `./configs/infer_configs`
For instance, to run the pre-trained model for intra-dataset evaluation on MMPD, execute:
```bash
python main.py --config_file ./configs/infer_configs/MMPD_MMPD_Q2FPhys.yaml
```


## 🎓 Acknowledgement
Our framework was implemented based on the [rPPG-Toolbox](https://github.com/ubicomplab/rPPG-Toolbox) [1], and additionally incorporates [RhythmMamba](https://github.com/zizheng-guo/RhythmMamba) [2] as a baseline model for comparison.



## References
[1] Liu, Xin, et al. "rppg-toolbox: Deep remote ppg toolbox." *Advances in Neural Information Processing Systems*, vol. 36, 2024.

[2] Zou, Bochao, et al. "Rhythmmamba: Fast remote physiological measurement with arbitrary length videos." *arXiv preprint* arXiv:2404.06483, 2024.
