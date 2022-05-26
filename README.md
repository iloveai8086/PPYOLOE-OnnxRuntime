# pp-yoloe-onnxruntime
克隆大佬的项目，原始仓库只给了代码，用makefile和onnxruntime cpp进行推理，推理为cpu端推理还未使用GPU

使用ONNXRuntime部署PP-YOLOE目标检测，支持PP-YOLOE-s、PP-YOLOE-m、PP-YOLOE-l、PP-YOLOE-x四种结构，包含C++和Python两个版本的程序

起初想使用OpenCV部署的，可是opencv的dnn模块读取onnx文件总是失败，于是只能使用onnxruntime部署了。
由于模型文件比较大，无法直接上传到仓库，因此把模型文件放在百度云盘里，下载
链接: https://pan.baidu.com/s/1wGwkQ2nzPmCZS8aXnZAB2Q  密码: krua

# 如何使用
```
1.在Makefile文件中修改你的opencv的路径
2.对于python端ort的推理，直接pip安装就行
3.对于CPP，需要make run，即可将推理的结果保存在workspace下
```

