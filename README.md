<p align="center">
    <img src="figs/logo.png" width="30%", style="vertical-align: middle; margin-right: 0px; position: relative; top: 25px;"> <br>

</p>

<div align="center">

# Flowing Fidelity to Detail for Efficient High-Resolution Video Generation


[![project page](https://img.shields.io/badge/Project_page-More_visualizations-green)](https://anonymous-researcher1.github.io/flashvideo-page/)&#160;

</div>

<div>

<p align="center">
<img src="figs/methodv3.png" width=90%>
<p>



## 🤗 More video examples 👀 can be accessed at the [![project page](https://img.shields.io/badge/Project_page-More_visualizations-green)](https://Anonymous-Researcher1.github.io/flashvideo-page/)


#### <span style="color:blue">⚡⚡</span> User Prompt to <span style="color:green">270p</span>, NFE = 50, Takes ~30s <span style="color:blue">⚡⚡
#### ⚡⚡</span>  <span style="color:green">270p</span> to <span style="color:purple">1080p</span> , NFE = 4, Takes ~72s <span style="color:blue">⚡⚡</span>

[![]()](https://github.com/Anonymous-Researcher1/flashvideo-page/blob/main/static/images/output.gif)




<p align="center">
<img src="https://github.com/Anonymous-Researcher1/flashvideo-page/blob/main/static/images/output.gif" width="100%"> <br>

</p>






## 🔥 🔥 🔥  Introduction
In this repository, we provide:

- [x] The stage-I weight for 270P video generation.
- [x] The stage-II for enhancing 270P video to 1080P.
- [x] Inference code of both stages.



## Install

### 1. Environment Setup

This repository is tested with PyTorch 2.4.0+cu121 and Python 3.11.11. You can install the necessary dependencies using the following command:

```shell
pip install -r requirements.txt
```

### 2. Preparing the Checkpoints



The checkpoints should be organized as shown below:

```
├── 3d-vae.pt
├── stage1.pt
└── stage2.pt
```

## 🚀 Text to Video Generation

#### ⚠️ IMPORTANT NOTICE ⚠️  :  Both stage-I and stage-II are trained with long prompts only. For achieving the best results, include comprehensive and detailed descriptions in your prompts, akin to the example provided in [example.txt](./example.txt).

### Jupyter Notebook

You can conveniently provide user prompts in our Jupyter notebook. The default configuration for spatial and temporal slices in the VAE Decoder is tailored for an 80G GPU. For GPUs with less memory, one might consider increasing the spatial and temporal slice.


```python
flashvideo/demo.ipynb
```

### Inferring from a Text File Containing Prompts

You can conveniently provide the user prompt in a text file and generate videos with multiple gpus.

```python
bash inf_270_1080p.sh
```

## License

This project is developed based on [CogVideoX](https://github.com/THUDM/CogVideo). Please refer to their original [license](https://github.com/THUDM/CogVideo?tab=readme-ov-file#model-license) for usage details.



