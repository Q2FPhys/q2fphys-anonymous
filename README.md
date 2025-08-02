## Overview of Q2F-Phys
(The code will be released soon.)
Q2F-Phys: A Label-Quantized Coarse-to-Fine Framework for Robust and Efficient Physiological Measurement
<p align="center">
  <img src="assets/figures/Overview.png" alt="Framework Overview" width="800"/>
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
This work builds upon the [rPPG-Toolbox](https://github.com/ubicomplab/rPPG-Toolbox) [1].  
We sincerely thank the authors for providing this valuable resource to the community.



## References
[1] Liu, Xin, et al. "rppg-toolbox: Deep remote ppg toolbox." *Advances in Neural Information Processing Systems*, vol. 36, 2024.
