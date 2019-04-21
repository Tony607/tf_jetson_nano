# Run Keras/Tensorflow model on Jetson Nano


## How to Run
Require [Python 3.5+](https://www.python.org/ftp/python/3.6.7/python-3.6.7.exe) and [Jupyter notebook](https://jupyter.readthedocs.io/en/latest/install.html) installed
### Clone or download this repo
```
git clone https://github.com/Tony607/tf_jetson_nano
```

### Install required libraries for your development machine
`pip3 install -r requirements.txt`
## A. The Keras Image classification model
[How to run Keras model on Jetson Nano](https://www.dlology.com/blog/how-to-run-keras-model-on-jetson-nano/) | DLology Blog
### Step1: Convert Keras model into TensorRT model
On development machine or [Google Colab](https://colab.research.google.com/github/Tony607/tf_jetson_nano/blob/master/Step1_Colab_TensorRT.ipynb)


To run locally, start a terminal, then run,
```
jupyter notebook
```

In the opened browser window open
```
Step1_Colab_TensorRT.ipynb
```

### Step2: Make prediction (On Jetson Nano)
To run notebook on Jetson Nano and make it accessible from another machine, in its terminal run,
```
jupyter notebook --ip=0.0.0.0
```
In another machine's browser, open the notebook,
```
http://<Jetson Nano's LAN IP address>:8888/notebooks/Step2_keras-jetson-ImageNet-predict.ipynb
```
## B.Tensorflow object detection model
[How to run TensorFlow Object Detection model on Jetson Nano](https://www.dlology.com/blog/how-to-run-tensorflow-object-detection-model-on-jetson-nano/) | DLology Blog

### Step1: Convert Tensorflow object detection model into TensorRT model 
On development machine or [Google Colab Notebook](https://colab.research.google.com/github/Tony607/tf_jetson_nano/blob/master/Step1_Object_detection_Colab_TensorRT.ipynb)

To run locally, start a terminal, then run,
```
jupyter notebook
```

In the opened browser window open
```
Step1_Object_detection_Colab_TensorRT.ipynb
```

### Step2: Make prediction (On Jetson Nano)
To run notebook on Jetson Nano and make it accessible from another machine, in its terminal run,
```
jupyter notebook --ip=0.0.0.0
```
In another machine's browser, open the notebook,
```
http://<Jetson Nano's LAN IP address>:8888/notebooks/Step2_jetson-object-detection-predict.ipynb
```