# Object Tracking using YOLOv5, Deep Sort ,bird view using depth estimation and Prediction using UKF
This repository implements a ROS2 Node contains YOLO5 Deep SORT in order to perfrom real-time object tracking. Yolov5 is an algorithm that uses deep convolutional neural networks to perform object detection. We can feed these object detections into Deep SORT (Simple Online and Realtime Tracking with a Deep Association Metric) in order for a real-time object tracker to be created. Then subscribe to a depth image from zed2 camera or any other depth estimation method to get the bird view then predict the motion of objects using UKF.

yolo3 and yolo5 were tested on this code, you can use any.

## project pipeline:

### detection


![detection](gif/det.gif)






### tracking


![tracking](gif/tracking.gif)







### bird view using depth image


![bird view using depth image](gif/bird_view.gif)






### prediction


![prediction](gif/pred1.gif)






### prediction


![prediction](gif/pred2.gif)

## Getting started

#### Conda (Recommended)
conda create -n <env_name> python=3.8

then install all requirements in yolo5 requirements file

#### to run 

python object_tracker_node_depth.py

##### for depth estimation you can use zed2 camrea for high accuracy but if you do not have you can use the ros2 node in this link

https://github.com/michaelhesham/Self-Driving-vehicles-course/tree/master/Graduation_project/monodepth2

## Acknowledgments
* [yolov5 torch](https://github.com/ultralytics/yolov5)
* [Yolov3 TensorFlow Amazing Implementation](https://github.com/zzh8829/yolov3-tf2)
* [Deep SORT Repository](https://github.com/nwojke/deep_sort)
* [Yolo v3 official paper](https://arxiv.org/abs/1804.02767)
