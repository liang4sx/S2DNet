# Delving into Details: Synopsis-to-Detail Networks for Video Recognition (S2DNet)

This repo is the official Pytorch implementation of our paper:
> [Delving into Details: Synopsis-to-Detail Networks for Video Recognition]()  
> Shuxian Liang, Xu Shen, Jianqiang Huang, Xian-Sheng Hua   
> ECCV 2022 Oral   

![s2dnet](s2dnet.jpg)

*Comming soon*

## Prerequisites

The code is built with following libraries:

- [PyTorch](https://pytorch.org/) 1.10.0 or higher 
- [Torchvision](https://github.com/pytorch/vision)
- [TensorboardX](https://github.com/lanpa/tensorboardX)
- [tqdm](https://github.com/tqdm/tqdm.git)
- [scikit-learn](https://scikit-learn.org/stable/)
- [ffmpeg](https://www.ffmpeg.org/)

## Data Preparation

Our work uses [Kinetics](https://www.deepmind.com/open-source/kinetics) and Something-Something V1&V2 for evaluation. We first extract videos into frames for fast reading. Please refer to [TSN](https://github.com/yjxiong/temporal-segment-networks) and [TSM](https://github.com/mit-han-lab/temporal-shift-module) repositories for the detailed guide of data pre-processing.

- Extract frames from videos
- Generate annotations needed for dataloader
- Add the information to [ops/dataset_configs.py](ops/dataset_configs.py)

For Mini-Kinetics dataset used in our paper, you need to use the train/val splits file from [AR-Net](https://github.com/mengyuest/AR-Net).

## Acknowledgement
Our code is built using [TSM](https://github.com/mit-han-lab/temporal-shift-module) and [SlowFast](https://github.com/facebookresearch/SlowFast) repositories.


## Citing
If you find our code or paper useful, please consider citing

    @inproceedings{liang2022delving,
        title={Delving into Details: Synopsis-to-Detail Networks for Video Recognition},
        author={Shuxian Liang, Xu Shen, Jianqiang Huang, Xian-Sheng Hua},
        booktitle={European Conference on Computer Vision},
        year={2022}
    }

