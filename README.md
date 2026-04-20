# CD2P-Net

PyTorch implementation for dual-polarization SAR despeckling with multitemporal observations.

**Authors:** Jiangong Xu, Yang Yang, Weibao Xue, Xiaoyu Yu, Junli Li, Jun Pan, and Mi Wang

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-1.9%2B-red)

---

## Overview

This repository provides the official implementation of **CD2P-Net**, a deep learning framework developed for despeckling real Sentinel-1 dual-polarization SAR imagery under multitemporal conditions.

CD2P-Net is designed to make use of neighboring temporal observations together with dual-polarization feature representations. The model combines spatial and frequency-aware feature processing and is built for unsupervised training on noisy SAR data, without requiring clean reference images.

The current project focuses on:

- multitemporal learning for SAR despeckling
- dual-polarization feature modeling
- physically meaningful representation design
- evaluation on real Sentinel-1 time-series data

---

## Main Characteristics

- Supports despeckling of **real dual-polarization Sentinel-1 SAR images**
- Uses **adjacent temporal acquisitions** during learning
- Incorporates **covariance-derived and decomposition-related features**
- Implements a **dual-domain network architecture**
- Trained in an **unsupervised** manner on noisy observations

---

## Repository Contents

```text
CD2P-Net/
├── data/           # dataset organization and preprocessing files
├── models/         # network definitions
├── train.py        # training script
├── test.py         # inference / evaluation script
├── utils/          # utility functions
└── README.md
```

> Update the file structure above if your repository uses different folder names.

---

## Dataset

The experiments are based on real Sentinel-1 dual-polarization SAR time-series data.
Please organize the dataset according to the structure required by the training and testing scripts.

If the dataset link is public, you can provide it here:

- Dataset: `TBD`
- Preprocessing instructions: `TBD`

---

## Environment

Recommended environment:

- Python 3.8+
- PyTorch 1.9+
- CUDA-enabled GPU for training

Install dependencies with:

```bash
pip install -r requirements.txt
```

---

## Training

Run the training script with:

```bash
python train.py
```

You may modify the configuration files or script arguments to set:

- data paths
- batch size
- learning rate
- checkpoint directory
- training epochs

---

## Testing

Run inference or evaluation with:

```bash
python test.py
```

Please make sure that the pretrained weights and dataset paths are correctly specified before testing.

---

## Pretrained Weights

Pretrained models will be released here:

- `TBD`

---

## Citation

If you find this repository useful in your research, please cite the corresponding paper.

```bibtex
@article{xu2026cd2pnet,
  title={Physically consistent multitemporal dual-domain learning for dual-polarization SAR despeckling},
  author={Xu, Jiangong and Yang, Yang and Xue, Weibao and Yu, Xiaoyu and Li, Junli and Pan, Jun and Wang, Mi},
  journal={International Journal of Applied Earth Observation and Geoinformation},
  year={2026},
  note={under review}
}
```

> If the paper is not yet publicly available, you may also temporarily remove the BibTeX block and keep only a plain-text citation note.

---

## Acknowledgements

We thank the providers of Sentinel-1 data and the open-source community for tools that supported this implementation.

---

## Contact

For questions regarding the code, please contact:

- Jiangong Xu: `dd_xjg@whu.edu.cn`
