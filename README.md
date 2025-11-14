## **Team Member**

**Name:** Atharv Sahu
**Roll Number:** 23MIA1153

# [Siggraph Asia 2023] Low-light Image Enhancement with Wavelet-based Diffusion Models

Hai Jiang<sup>1,2</sup>, Ao Luo<sup>2</sup>, Haoqiang Fan<sup>2</sup>, Songchen Han<sup>1</sup>, Shuaicheng Liu<sup>3,2</sup>

1. Sichuan University, 2. Megvii Technology, 3. University of Electronic Science and Technology of China

## Pipeline

![](./Figures/pipeline.png)

## Dependencies

```
pip install -r requirements.txt
```

## Download the raw training and evaluation datasets

### Paired datasets

LOLv1 dataset: Chen Wei, Wenjing Wang, Wenhan Yang, and Jiaying Liu. "Deep Retinex Decomposition for Low-Light Enhancement", BMVC, 2018.
Baiduyun (extracted code: sdd0)
Google Drive

LOLv2 dataset: Wenhan Yang, Haofeng Huang, Wenjing Wang, Shiqi Wang, and Jiaying Liu. "Sparse Gradient Regularized Deep Retinex Network for Robust Low-Light Image Enhancement", TIP, 2021.
Baiduyun (extracted code: l9xm)
Google Drive

LSRW dataset: Jiang Hai, Zhu Xuan, Ren Yang, Yutong Hao, Fengzhu Zou, Fang Lin, and Songchen Han. "R2RNet: Low-light Image Enhancement via Real-low to Real-normal Network", Journal of Visual Communication and Image Representation, 2023.
Baiduyun (extracted code: wmrr)

### Unpaired datasets

Refer to Project Page of RetinexNet.

## Pre-trained Models

Download from Google Drive or Baidu Yun (extracted code: wsw7).

## How to train?

Modify `datasets/dataset.py` for your environment:

```
python train.py
```

## How to test?

```
python evaluate.py
```

## Visual comparison

![](./Figures/comparison.png)

## Citation

```
@article{jiang2023low,
  title={Low-light image enhancement with wavelet-based diffusion models},
  author={Jiang, Hai and Luo, Ao and Fan, Haoqiang and Han, Songchen and Liu, Shuaicheng},
  journal={ACM Transactions on Graphics (TOG)},
  volume={42},
  number={6},
  pages={1--14},
  year={2023}
}
```

## Acknowledgement

Part of the code is adapted from WeatherDiff, SDWNet, and MIMO-UNet. We thank all the authors for their contributions.
