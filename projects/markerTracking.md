---
layout: post
title: Head Motion Tracking using Marker
permalink: /projects/markerTracking
---

Work done under the guidence of [Dr. Ehtesham Hassan](https://www.linkedin.com/in/ehtesham-hassan-b9a8aa2/).
<p>
<img src="/images/Fig1.png" style="width:300px;height:146px;" align="right">
The marker tracking method for forehead motion analysis is non invasive approach for behavior modeling and hence can be used in Video analytics and Medical Diagnosis for Nuero-development disorders. For the online diagnosis, the setup consists of single monocular camera for feeding in the visual input, which focuses on head movements of the subject taking the diagnostic test. The head movements are captured by tracking an active marker worn at subject’s forehead. In this setup, we have used circular marker made up of green color. In the testing process, a stimuli is played on the computer screen, where camera captures the face of the subject exhibiting various responses while performing actions in response to the stimuli on the screen.
</p>

We ovecome two primary challenges. First, accuracy as the behavior analysis outcome depends on the precision and accuracy of detected track. Second, the processing needs to time efficient addressing both the scenarios offline and online detection without compromising the accuracy. To address this problem, we present a monocular tracking scheme for frame-wise detection of non-textured active color marker observed from on/off axis angle. The frame level detection targets high precision and accuracy, whereas we exploit the motion information for reducing search space in subsequent frames and the fact of marker's circularity for improving the timing performance.


<p><img src="/images/overview.png" style="width:300px;height:100px;" align="right">
 There are two major steps involved in the whole process. The first part used is detection of an accurate location of circular marker and do an online learning of it. The detection is solely based on information of marker color and knowledge od marker's cicularity, which always gives accrate results but very time consuming. Hence, it generates important features of the object at this step. The same module is used for updating the training data also. The second step is pixel wise classification using trained SVM on features form the first step. This process independently works for detection process in further frames. This step also uses the motion information for getting Region of Interest in subsequent frames. Also we downsample followed by upsample on marker's boundary to reduce number of test pixels.
</p>
Refer to filed [Patent](http://www.freepatentsonline.com/y2017/0278266.html) for more info.

