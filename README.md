# GraM-Diff: A Unified Graph–Mamba Diffusion Framework for EEG-Based Alzheimer’s Disease Data Generation and Diagnosis

> **Accepted (Oral)** at the **MICCAI Student Board 2026 EMERGE Workshop** — *Empowering Medical Information Computing and Research through Early-career Guidance and Expertise*.

> **Abstract:** Electroencephalography (EEG) is a promising, non-invasive, and cost-effective modality for Alzheimer’s disease (AD) detection, but deep learning methods are limited by small and imbalanced clinical datasets. Generative augmentation offers a solution, yet existing approaches rely on inefficient class-specific models or fail to capture complex spatial and temporal brain dynamics. To address this, we propose GraM-Diff, a unified classifier-guided Graph–Mamba diffusion framework
for EEG synthesis. It embeds Graph Convolutional Networks within a diffusion U-Net to model inter-electrode connectivity and Bidirectional Mamba state-space blocks for linear-complexity long-range temporal modeling. Latent-space classifier guidance lets a single model generate both healthy and pathological EEG within a shared representation, avoiding fragmented per-cohort pipelines. Across four EEG-based AD benchmarks, synthetic augmentation improves classification, yields superior
Context-FID and correlation scores over strong generative baselines, and enhances robustness in data-scarce settings.

## Authors

[M. Tanveer](mtanveer@iiti.ac.in), [Ayush Singh Rana](cse240001015@iiti.ac.in), [Sanskriti Jain](cse240001064@iiti.ac.in), [Arnav Kumar](cse240001013@iiti.ac.in), [Aryaman Tiwari](cse240001014@iiti.ac.in), [Abdur Rahaman](phd2401141001@iiti.ac.in), [Abdul Quadir](mscphd2207141002@iiti.ac.in), [M. Sajid](phd2101241003@iiti.ac.in)

## Publication

This work has been accepted as an **Oral presentation** at the **MSB EMERGE 2026** workshop (MICCAI Student Board).

## Requirements

The dependencies can be installed by:

```bash
pip install -r requirements.txt
```

## How to Run

Follow these steps to configure and run the framework:

1. **Prepare the Dataset**: Place the correct dataset into the `datasets` folder.
2. **Set Configurations**: Configure your config file correctly to match your dataset and training parameters.
3. **Train the Model**: Start the training process by running the `trainEEG` script:
```bash
python trainEEG.py
```

4. **Sample**: Once training is complete, generate your samples by running the `sample` script:
```bash
python sample.py
```

## Citation

If you find this work useful, please consider citing:

```bibtex
@inproceedings{gramdiff2026,
  title     = {GraM-Diff: A Unified Graph–Mamba Diffusion Framework for EEG-Based Alzheimer’s Disease Data Generation and Diagnosis},
  author    = {Tanveer, M. and Rana, Ayush Singh and Jain, Sanskriti and Kumar, Arnav and Tiwari, Aryaman and Rahaman, Abdur and Quadir, Abdul and Sajid, M.},
  booktitle = {MICCAI Student Board (MSB) EMERGE Workshop},
  year      = {2026}
}
```

