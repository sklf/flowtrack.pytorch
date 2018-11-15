# flowtrack.pytorch
Pytorch implementation of [FlowTrack](https://arxiv.org/pdf/1804.06208.pdf).

**Simple Baselines for Human Pose Estimation and Tracking** (https://arxiv.org/pdf/1804.06208.pdf)



### TO DO:

- [x] Human detection
- [x] Single person pose estimation
	- [x] Building
	- [x] Training
- [x] Optical flow estimation
- [x] Box propagation
- [ ] Pose tracking



### Requirements
```
Python2.7
Pytorch0.4.0
```
And for other requirements, you can refer to [pytorch-faster-rcnn](https://github.com/ruotianluo/pytorch-faster-rcnn) and [pytorch-faster-rcnn](https://github.com/ruotianluo/pytorch-faster-rcnn)
### Installation

```shell
cd lib
./make.sh
```



### Demo

#### Pose Estimation

Download [data folder](https://drive.google.com/drive/folders/1RqsY3ONtYlxQfLg2acJm36qTtqvHDCik?usp=sharing) as `$ROOT/data`.

```shell
python ./tools/pose/main.py
```



#### Detection

Download pretrained [detection model](https://drive.google.com/file/d/18PKsPqSBx7C940zz95siAKiI_6aSE5hO/view?usp=sharing) into `models/detection/`. Refer to [pytorch-faster-rcnn](https://github.com/ruotianluo/pytorch-faster-rcnn) for more information.

```shell
python ./tools/detection/demo.py
```

#### 

#### Optical Flow Estimation

Download pretrained [flownet](https://drive.google.com/file/d/17d0x6q3FZZCfHMz7vND8E78WIZreqito/view?usp=sharing) into `models/flownet/`. Refer to [flownet2-pytorch](https://github.com/NVIDIA/flownet2-pytorch) for more information.

```shell
python ./tools/flownet/demo.py --model Flownet2S --resume </path/to/model>
```

