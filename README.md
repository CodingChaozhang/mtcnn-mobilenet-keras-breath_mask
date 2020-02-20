# mtcnn+mobilenet-keras-breath_mask
基于MTCNN+MOBILENET的人体口罩佩戴检测

由于2020年新型冠状病毒，针对公共场合检测人员是否佩戴口罩，故用MTCNN+MOBILENET完成一个人体口罩佩戴检测。

## 流程

 - 1.用MTCNN检测出人脸
 - 2.将人脸送入MobileNet进行校验是否带口罩

## 效果展示

![mask_sample](data/video/2.mkv)

## 环境

`工欲善其事必先利其器`

- **Python：** 3.7.4
- **Tensorflow-GPU：**1.14.0
- **Keras:** 2.2.4


## 训练步骤

 - 1.准备图片，放入data/image/train

 - 2.在根目录下，运行 `train.py` 进行训练mobilenet网络。可以根据情况修改 `train.py` 中的参数。

 - 3.在根目录下，运行 `mask_recognize.py`，可测试本地视频，当然也可以开启视频流



