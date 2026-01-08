# FluencyVE: Marrying Temporal-Aware Mamba with Bypass Attention for Video Editing

[![arXiv](https://img.shields.io/badge/arXiv-2512.21015-b31b1b.svg)](https://arxiv.org/abs/2512.21015)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

Official PyTorch implementation of **FluencyVE**, accepted by **IEEE Transactions on Multimedia (TMM)**.

## 🌟 Highlights

- **Temporal-Aware Mamba**: Linear complexity O(N) for efficient global frame attention
- **Bypass Attention**: 94% parameter reduction while maintaining generative quality
- **One-Shot Editing**: Edit videos with minimal training
- **Superior Performance**: Better temporal consistency and editing quality

## 📰 News

- **[2025-12]** 🎉 Paper accepted by IEEE Transactions on Multimedia!
- **[2025-12]** 📄 Paper available on [arXiv](https://arxiv.org/abs/2512.21015)
- **[2025-01]** 💻 Code and models released!

## 🚀 Quick Start

### Training-Free Video Editing

```bash
# Create environment
conda create -n fluencyve python=3.10
conda activate fluencyve
cd Tuning_free_MambaD
pip install -r requirements.txt

# DDIM inversion (preprocess your video)
python ddim_inversion.py

# Video editing
python dni.py
```

### Fine-Tuning Based Video Editing

```bash
# Create environment
conda create -n fluencyve_tuning python=3.10
conda activate fluencyve_tuning
cd Tuning_MambaD
pip install -r requirements.txt

# Model tuning
python dni_tuning.py

# Video editing
python dni.py
```

## 📖 Citation

If you find this work useful, please cite our paper:

```bibtex
@article{cai2025fluencyve,
  title={FluencyVE: Marrying Temporal-Aware Mamba with Bypass Attention for Video Editing},
  author={Cai, Mingshu and Li, Yixuan and Yoshie, Osamu and Ieiri, Yuya},
  journal={arXiv preprint arXiv:2512.21015},
  year={2025}
}
```

## 🙏 Acknowledgements

This work is supported by Waseda University and Southeast University. We thank the authors of [Stable Diffusion](https://github.com/CompVis/stable-diffusion), [Tune-A-Video](https://github.com/showlab/Tune-A-Video), and [Mamba](https://github.com/state-spaces/mamba) for their excellent work.

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
