# Bilinear-CNN-for-SCA

This repository contains data and examples for reproducing the results presented in "Improving Deep Learning Based Second-Order Side-Channel Analysis with Bilinear CNN". 

In this paper, we introduce a new architecture (called B-CNN) in the context of profiled SCA, which embeds the product combination of leakage into neural networks. We further propose a novel visualization tool (called LWC) that helps to interpret and understand the inner-working and decision-making of B-CNN. We show that B-CNN performs systematically better (w.r.t. the number of attack traces) than the current state-of-the-art results on all the investigated datasets (protected with masking countermeasure). The main structure of B-CNN is shown as bellow:

<div align="center">
	<img src="https://github.com/loccs-cp/Bilinear-CNN-for-SCA/raw/main/figure/B-CNN.jpg" alt="Editor" width="600">
</div>

## Datasets

Three side-channel datasets are investigated in this work:

### ASCAD FIXED KEY dataset
Information about ASCAD FIXED KEY dataset can be found in the original github page: [https://github.com/ANSSI-FR/ASCAD/tree/master/ATMEGA_AES_v1/ATM_AES_v1_fixed_key](https://github.com/ANSSI-FR/ASCAD/tree/master/ATMEGA_AES_v1/ATM_AES_v1_fixed_key)

### ASCAD RANDOM KEY dataset
Information about ASCAD RANDOM KEY dataset can be found in the original github page: [https://github.com/ANSSI-FR/ASCAD/tree/master/ATMEGA_AES_v1/ATM_AES_v1_variable_key](https://github.com/ANSSI-FR/ASCAD/tree/master/ATMEGA_AES_v1/ATM_AES_v1_variable_key)

### CHES CTF 2018 dataset
Information about CHES CTF 2018 dataset can be found in the CHES CTF 2018 website: [https://chesctf.riscure.com/2018/content?show=training](https://chesctf.riscure.com/2018/content?show=training)

The dataset (ches_ctf.h5 file) that we use was downloaded from: [https://www.dropbox.com/s/lpw1k3so99krmmq/ches_ctf.h5?dl=0](https://www.dropbox.com/s/lpw1k3so99krmmq/ches_ctf.h5?dl=0)

## Repository structure
This repository is composed of the following folders and script:

- **./Data:** the dataset (.npy format) used in the experiments. 
- **./models**: contains the trained model.
- **./\*.ipynb**: the notebook file that contains both codes and outputs. This notebook demonstrates how to load a dataset, how to pre-process the data, how to perform adversarial training, and how to evaluate the models, etc.

Note: If you cannot open the '*.ipynb' notebook in Github, please try to open it using the nbviewer online: [https://nbviewer.org/github/loccs-cp/Bilinear-CNN-for-SCA/blob/main/](https://nbviewer.org/github/loccs-cp/Bilinear-CNN-for-SCA/blob/main/)
