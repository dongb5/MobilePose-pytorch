# DeepPose-pytorch
Reproduce Google's [DeepPose](https://arxiv.org/pdf/1312.4659.pdf) with Resnet18 by Pytorch

## Functionality

1. **Tiny** trained model (<10MB)
2. **Fast** inference speed (>30FPS)
3. **Accurate** keypoint estimation (~40mAP)

## Requirements:
- Python 3.6.2
- Pytorch 0.2.0\_3 

## Todo List:
- [x] accuracy(mAP) evaluation script
- [x] multi-scales training
- [x] data augmentation(rotate/shift/flip/multi-scale)
- [x] support LSP dataset
- [x] normalization(/256 mean std)
- [x] adding weighted loss(coco keypoints weight) 
- [x] support Macbook camera realtime skeleton display demo

## Usage

1. Resnet18 Training(~40MB):
```shell
python training.py
```
2. MobilenetV2 Training(~9MB):
```shell
python training-mobilenetv2-czx.py
```
3. Evaluation
```shell
python eval-coco-add2dim.py
```

4. Realtime visualization:
```shell
python realtime_webcam.py
```

