## Introduction

A state of art detector for densely packed scenes dataset SKU-110K.

For more information, please read our technical report, [https://arxiv.org/pdf/2007.11946](https://arxiv.org/pdf/2007.11946)

<img src="preview.jpg" alt="avatar" style="zoom: 33%;" />

## License

This project is released under the [Apache 2.0 license](https://github.com/Media-Smart/vedacls/blob/master/LICENSE).

## Installation

1. To clone this project to your own device.

   ```
   git clone https://github.com/Media-Smart/SKU110K-DenseDet.git
   ```

2. Please refer to [INSTALL.md](docs/INSTALL.md) for installation and dataset preparation.

3. Click [here](https://drive.google.com/file/d/1XM8OzRdcbDbSrvlcMgJsFX76lBmdN2Td/view?usp=sharing) to download the weights. 

## Get Started

Please go to [GETTING_STARTED.md](docs/GETTING_STARTED.md) for the basic usage of MMDetection.

Before you are about to run or train, please edit the path in  [configuration](configs/SKU_fusion_bifpn_x101_32x4d.py)

### Test

```shell
python tools/test.py configs/SKU_fusion_bifpn_x101_32x4d.py \
    ${YOUR_WEIGHT_PATH} \
    --show
```

### Train

```shell
python tools/train.py configs/SKU_fusion_bifpn_x101_32x4d.py
```

## Performance

The performance applied on SKU-110k of our best solution.

|            | mAP   | AP@50  | AP@75 |
| ---------- | ----  | -----  | ----- |
| Val Set    | 58.0% | 92.0%  | 66.5% |
| Test Set 1 | 58.7% | 92.9%  | 67.3% |

For more detail, please browse the [configuration](configs/SKU_fusion_bifpn_x101_32x4d.py)

## Contact

This repository is currently maintained by Tianze Rong ([@SteelBeamR](https://github.com/SteelBeamR)), Hongxiang Cai ([@hxcai](http://github.com/hxcai)), Yichao Xiong ([@mileistone](https://github.com/mileistone)).

## Credits

The whole project is based on  [mmcv v0.5.9](https://github.com/open-mmlab/mmcv/tree/v0.5.9) and [mmdetection v1.0rc1](https://github.com/open-mmlab/mmdetection/tree/v1.0rc1) via [open-mmlab](https://github.com/open-mmlab).

