# Repository Organisation and Etiquette 

## SUCS Repository

This system is composed of 3 parts, the main server, the image analysis server and the front-end system(the SUCS website).

Python is used to develop the main server and the image analysis server. HTML, CSS, Javascript are used to develop the front-end system.

**The front-end system** is the web interface.

**The main server** is the middle layer connecting the database, frontend system, image analysis server and map engine provided by Baidu, Google and OpenStreetView. 

**The image analysis server** is responsible for running image analysis algorithm.


## Utility Detection Model Training Repository 

The detection model in SUCS is based on Faster-RCNN detection algorithm and ResNet-50 deep neural network.

Through training with a dataset of 1299 manhole cover images, the detection accuracy of the model reaches 76.7% on the testset. SUCS just uses this model.

For your convenience, please check [Utility Detection Tool](https://github.com/yehan-xiao/utility-detection-tool.git) to see the details of training deep-learning model.