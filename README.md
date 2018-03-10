## READ TO ME
这个项目我只看了代码，并没有实际训练，因为没有导入imagenet的预训练模型，大概效果不会好，而且issues提到很多没有训练成功的。

代码也是看的一知半解，用到了slim的库，涉及到张量的问题有点迷糊==

主要参考链接：
[CSDN](http://blog.csdn.net/qq_34784753/article/details/78803423)
[知乎](https://zhuanlan.zhihu.com/p/25053311)
[IoU](https://www.lao-wang.com/?p=114)


## YOLO_tensorflow

Tensorflow implementation of [YOLO](https://arxiv.org/pdf/1506.02640.pdf), including training and test phase.

### Installation

1. Clone yolo_tensorflow repository
	```Shell
	$ git clone https://github.com/hizhangp/yolo_tensorflow.git
    $ cd yolo_tensorflow
	```

2. Download Pascal VOC dataset, and create correct directories
	```Shell
	$ ./download_data.sh
	```

3. Download [YOLO_small](https://drive.google.com/file/d/0B5aC8pI-akZUNVFZMmhmcVRpbTA/view?usp=sharing)
weight file and put it in `data/weight`

4. Modify configuration in `yolo/config.py`

5. Training
	```Shell
	$ python train.py
	```

6. Test
	```Shell
	$ python test.py
	```

### Requirements
1. Tensorflow

2. OpenCV
