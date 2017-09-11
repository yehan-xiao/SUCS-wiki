# Constraints 

## Street view images can not cover all roads

SUCS will not be able to scan all roads, as this is dependent on the available street view images.  Street view images for roads in derelict regions are sparse and only tend to follow major roads, whereas well developed towns and cities will include street view images for almost all public roads.


## Street view images may be out of date

As the cities are always expanding and developing, the data of utilities are out of date. For instance, the street images of Baidu in Ningbo were collected in 2014. Also, we can not make sure the images will be updated at regular intervals.


## Utilities may be detected more than once or be missed

In a road, there are nearly infinite street view images. The approach of picking up images is very important. If two adjacent images have same part, the utilities will count twice. But if they are too far away, it will have utilities missing.


## Utilities have variable degrees of distortion

Since the street view images are taken by cameras from a series of distance, objects on images will have different degrees of distortion, which is the biggest challenge to the accuracy of deep learninng.

We have try our best to collect the training dataset mixed all kinds of distortion to enable the model flexible.