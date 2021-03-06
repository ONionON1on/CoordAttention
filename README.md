# Coordinate Attention for Efficient Mobile Network Design ([preprint](https://arxiv.org/abs/2103.02907))

This repository is a PyTorch implementation of our coordinate attention (will appear in CVPR2021).

Our coordinate attention can be easily plugged into any classic building blocks as a feature representation augmentation tool. Here ([pytorch-image-models](https://github.com/rwightman/pytorch-image-models)) is a code base that you might want to train a classification model on ImageNet.


### Comparison to Squeeze-and-Excitation block and CBAM

![diagram](diagram.png)

(a) Squeeze-and-Excitation block      (b) CBAM      (C) Coordinate attention block


### How to plug the proposed CA block in the [inverted residual block](https://openaccess.thecvf.com/content_cvpr_2018/papers/Sandler_MobileNetV2_Inverted_Residuals_CVPR_2018_paper.pdf) and the [sandglass block](https://arxiv.org/pdf/2007.02269.pdf)

![wheretoplug](attpos.png)

(a) MobileNetV2 (b) MobileNeXt

### Object detection

We use this [repo (ssdlite-pytorch-mobilenext)](https://github.com/Andrew-Qibin/ssdlite-pytorch-mobilenext).

### Semantic segmentation

We use this [repo](https://github.com/Andrew-Qibin/SPNet). You can also refer to [mmsegmentation](https://github.com/open-mmlab/mmsegmentation) alternatively.

### Citation

You may want to cite:

```
@inproceedings{hou2021coordinate,
  title={Coordinate Attention for Efficient Mobile Network Design},
  author={Hou, Qibin and Zhou, Daquan and Feng, Jiashi},
  booktitle={CVPR},
  year={2021}
}

@inproceedings{sandler2018mobilenetv2,
  title={Mobilenetv2: Inverted residuals and linear bottlenecks},
  author={Sandler, Mark and Howard, Andrew and Zhu, Menglong and Zhmoginov, Andrey and Chen, Liang-Chieh},
  booktitle={Proceedings of the IEEE conference on computer vision and pattern recognition},
  pages={4510--4520},
  year={2018}
}

@inproceedings{zhou2020rethinking,
  title={Rethinking bottleneck structure for efficient mobile network design},
  author={Zhou, Daquan and Hou, Qibin and Chen, Yunpeng and Feng, Jiashi and Yan, Shuicheng}
  booktitle={ECCV},
  year={2020}
}
```
