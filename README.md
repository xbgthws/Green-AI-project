## Green AI project Introduction
This repository stores code and project files related to the "Project Module" of THWS. The project name is "Green AI". Our group has tried to prune the YOLOv5 model and replace the backbone network to improve the reasoning efficiency of YOLOv5 and reduce the model size.

The original YOLOv5 code:[YOLOv5](https://github.com/ultralytics/yolov5/)(V6)

### 1.Replacement of the YOLOv5 backbone network
Replacing the backbone network in YOLOv5 involves substituting the default backbone with an alternative neural network architecture to potentially improve performance and efficiency.In our project, we tried to replace the backbone network with [MobileNetV2/V3](https://arxiv.org/abs/1704.04861),[GhostNet](https://arxiv.org/abs/1911.11907),[ShuffleNet](https://arxiv.org/abs/1707.01083) respectively.

1. Replacement of backbone network with Mobilenet
        ```
        python train.py --data coco.yaml --cfg yolov5s.yaml --weights '' --batch-size 32 --device 0 --epochs 300 --name coco --optimizer AdamW --data data/coco.yaml
        ```
## Authors：Bangguo Xu & Simei Yan & Liang Liu
