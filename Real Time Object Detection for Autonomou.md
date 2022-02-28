Real Time Object Detection for Autonomous Vehicles Using Deep Learning


(1.1) Object detection for autonomous vehicles

Autonomous driving technologies aim at navigating the road network without human intervention by sensing and reacting to the vehicle’s surrounding environment . This includes many challenges for Computer Vision and Deep Learning, such as object detection. Object detection is one of the most important requirements for autonomous navigation and consists of localization and classifcation of objects. Therefore, accurate object detection algorithms are needed. Recent state-of-the-art deep learning models that address the problem of object detection include Region-Based Convolutional Neural Networks (R-CNN) and their improved versions Fast R-CNN and Faster R-CNN, designed for model performance and first introduced in 2013. A second model for object detection introduced in 2015 is YOLO, designed for speed and real-time use

(1.1.1.) The critical tasks

object detection, 
Drivable area segmentation and 
lane detection

(1.1.2.) The visual perception system needed to perform the critical tasks(1.1.2.) The visual perception system needed to perform the critical tasks

THE VISUAL PERCEPTION SYSTEM plays a significant role in autonomous driving, as it can extract visual information from the images taken by the camera and assist the decision system to control the actions of the vehicle. In order to restrict the manoeuvre of vehicles, the visual perception system should be able to understand the scene and then provide the decision system with information including locations of the obstacles, judgements of whether the road is drivable, the position of the lanes etc.

(1.1.2.1.) OBJECT DETECTION is usually involved in the driving perception system to help the vehicles avoid obstacles and follow traffic rules. Drivable area segmentation and lane detection are also needed as they are crucial for planning the driving route of the vehicle

(1.1.2.2.) CRITICAL REQUIREMENTS. For such a visual perception system, high precision and real-time are two most critical requirements, which are related to whether the autonomous vehicle can make accurate and timely decision to ensure safety

(1.1.2.3.) CHALLENGES. it can be very challenging to take both requirements into account in real-world scenarios. Many methods handle these three critical tasks separately. For instance, while the Faster R-CNN-series and the YOLO-series deal with object detection, ENet and and PSPNet, are proposed to perform semantic segmentation. SCNN and SAD-ENet are used for detecting lanes

(1.1.2.4) PRELIMINARY CONCLUSION. Despite the excellent performance these methods have been able to achieve, processing these tasks one after another takes longer time than tackling them all at once. . Therefore, it is essential to explore multi-task approaches in autonomous driving. This exploration entails to solve the multi-task problem for the visual perception system, that is, object detection, drivable area segmentation and lane detection, while obtaining high precision and fast speed. 

But, we will not tackle the multi-task problem now. Instead, we will focus on the first critical task of the visual perception system, namely, traffic object detection

(1.2.) The Berkeley DeepDrive (BDD100K) Dataset

BDD100K, is the largest driving video dataset with 100K videos and 10 tasks to evaluate the progress of image recognition algorithms on autonomous driving. The dataset possesses geo-graphic, environmental, and weather diversity, which is useful for training models that are less likely to be surprised by new conditions. Provided are bounding box annotations of 13 categories for each of the reference frames of 100K videos and 2D bounding boxes annotated on 100.000 images for "other vehicle", "pedestrian", "traffic light", "traffic sign", "truck", "train", "other person", "bus", "car", "rider", "motorcycle", "bicycle", "trailer".

(1.3.) Approach and project goal

The goal of our project is to detect and classify traffic objects in a video in real-time using two approaches. We would train the two state-of-the-art models YOLO and Faster R-CNN on the Berkeley DeepDrive dataset to compare their performances.

(2)	Related work

(2.1) Traffic Object Detection models and Algorithms
