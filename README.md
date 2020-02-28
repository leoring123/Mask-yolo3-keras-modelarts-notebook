# Mask-yolo3-keras-modelarts-notebook
# 袁覃的建行云工作室
![袁覃的建行云工作室](https://github.com/leoring123/Mask-yolo3-keras-modelarts-notebook/blob/master/cloudccb.png)
大家好，我是建行常德桥南支行的客户经理袁覃。
同时，也是建行无感支付课题组成员。
曾借调建信金科，全流程参与了劳动者港湾人工智能垃圾分类模型的开发。
![华为云直播](https://github.com/leoring123/Mask-yolo3-keras-modelarts-notebook/blob/master/together.jpg)
![华为云Modelarts](https://github.com/leoring123/Mask-yolo3-keras-modelarts-notebook/blob/master/ma1.png)
---------------------------------------------------------------------------------------------------------------
传送门！！！
# ModelArts口罩佩戴模型开发直播课活动：
回看已出，参与活动及查看直播回放请点击：https://bbs.huaweicloud.com/forum/thread-42068-1-1.html
大家可以去练手！

开发指导文档https://github.com/huaweicloud/ModelArts-Lab/tree/master/contrib/1.%E5%8F%A3%E7%BD%A9%E6%A3%80%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%9B%B4%E6%92%AD%E5%BC%80%E5%8F%91%E6%8C%87%E5%AF%BC%E6%96%87%E6%A1%A3


# 防疫口罩佩戴检测模型前传！ 纪念华为云口罩佩戴检测模型直播圆满成功！助力防疫从你我做起，从小事做起！

The test environment is
    - Modelarts notebook
    - Python 3.5.2
    - Keras 2.1.5
    - tensorflow 1.6.0

# 无感支付技术与应用研究的光学识别理论延伸
  无感支付的概念界定：
--无感支付是用某种独一无二的特征标的物绑定银行账户或支付工具，通过一系列技术加以识别该特征标的物，从而完成支付。    
--目前识别技术主要可划分为三类，即光学识别、声学识别、各类波的识别，这些技术为无感支付提供了基础的技术条件。
--常见的初代无感支付场景有ETC高速通行、机场物业车牌识别、刷脸支付等等新零售的支付环节。

# 建研无感支付课题组
![建研无感支付课题组](https://github.com/leoring123/Mask-yolo3-keras-modelarts-notebook/blob/master/universityccb1.png)

![建研无感支付课题组学习场景](https://github.com/leoring123/Mask-yolo3-keras-modelarts-notebook/blob/master/universityccb2.png)



##Introduction

A Keras implementation of YOLOv3 (Tensorflow backend) inspired by allanzelener/YAD2K.

---

## Quick Start

1. Download YOLOv3 weights from [YOLO website](http://pjreddie.com/darknet/yolo/).
2. Convert the Darknet YOLO model to a Keras model.
   Make sure you have run python convert.py -w yolov3.cfg yolov3.weights model_data/yolo_weights.h5
3. upload all fold and model to Modelarts notebook
   BIG fold copy exmple: “import moxing as mox
                          mox.file.copy('s3://kerasyolo3masks416or/kerasyolo3notebook/','/home/ma-user/work/')”
4. Run step1control.ipynb

```
wget https://pjreddie.com/media/files/yolov3.weights
python convert.py yolov3.cfg yolov3.weights model_data/yolo.h5
python yolo_video.py [OPTIONS...] --image, for image detection mode, OR
python yolo_video.py [video_path] [output_path (optional)]

positional arguments:
  --input        Video input path
  --output       Video output path

部署到本地摄像头记得修改yolo.py   # vid = cv2.VideoCapture(video_path) 为# vid = cv2.VideoCapture(0)
本方案除了借鉴其它开源大佬的资料和建议，底层思维来自建研无感支付课题组的无感支付识别技术光学识别理论延伸而来。
感谢建信金科移动金融团队和华为云modelarts团队的支撑与支持。部分来自互联网的信息如有侵权，请及时联系作者删减。
tel：+86-13203636335    e-mail：61167448@qq.com
未完待续...
口罩智能识别.MP4为华为云落地应用简示。
