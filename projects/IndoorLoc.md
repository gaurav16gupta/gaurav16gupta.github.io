---
layout: post
title: Indoor Localisation and Navigation on Augmented Reality Devices
permalink: /projects/IndoorLoc
---
<p>
<img src="/images/udpFigure.jpg" style="width:300px;height:330px;" align="right">
This project targets a localisation and navigation application using an AR device such as GG and GC in conjunction with an Android smartphone. Figure illustrates the client-server framework which has three vertical components. The client is basically an android wearable/hand-held device which is used only to fetch the scene-images in real-time, and the IMU data. It also serves as an interactive console for the user by showing the dynamic location of the navigator in the generated map. The server which is remotely located contains the processing unit for performing all computations on image and sensor data. The central vertical maintains the two-way communication between client and server.  
</p>

<p>
<img src="/images/ISMAR_GGLocNew.jpg" style="width:250px;height:400px;" align="right">
</p>
At the wearable device:

OpenCV camera fetches frames from camera and passes it along with image metadata, over to UDP transmission thread. IMU sensor generates acceleration (in the 2D plane of user’s path) and orientation sensor data to transmit over the network. Then, it receives the indoor map coordinates from the server for displaying on GG screen. 

At the server (processing unit):

The Visual Odometry makes use of Shi Tomasi descriptors, tracked over time by Lucas Kanade’s optical flow. The sensor data (acceleration) is used to complement visual odometry using EKF based sensor fusion which gives a combined decision on pose estimation. Condition (A) holds true only when current position is greater then previous position by atleast Δ; where Δ is computed empirically – is the least distance between previous and current landmark where loop closure is not detected. Finally, loop closure detection is demonstrated as shown in the last block. 

This work was published at [ISMAR-2016](http://www.ismar.vgtc.org/). For detailed explaination refer [Paper](https://gaurav16gupta.github.io/papers/IndoorLocalisation.pdf).


