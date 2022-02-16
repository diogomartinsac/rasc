---
layout: post-page
title: Computer Vision
subtitle: Basic Concepts and Practical Examples
cover-img: /assets/img/2022-02-15-computer-vision-basics/cover.jpg
thumbnail-img: /assets/img/2022-02-15-computer-vision-basics/cover.jpg
share-img: /assets/img/rosa-logo-redondo.png
author: Israel Motta and Diogo Martins
comments: false
tags:
---

In this article are gathered some concepts for learning what computer vision is, and how to make computers able to visualize images and interpret the information contained in them, which is already an intrinsic capacity of the human being.

This introduction covers areas such as digital image processing, deep learning, camera calibration, and the use of fiducial markers. In each of these areas, some concepts are discussed and some techniques involved are demonstrated using Python. 


### Basic Concepts



In this practical mini course in computer vision for beginners, you will be introduced to approaches used to solve the task of pattern recognition in images, visualizing the challenges encountered, applications and the subdivisions of recognition in computer vision.

During the course we will analyze and process images. First, we'll look at the properties of images and explore the different image processing commands. After learning the basics, we will go through some exercises of identifying objects in images.

<center>
  <img src="{{ 'assets/img/2022-02-15-computer-vision-basics/basics.png' | relative_url }}" width="600" text-align=center alt="img1" />
</center>


[Colab](https://drive.google.com/file/d/1llBM5qg1iFfzHuy12C9C9a24Yp47-R8A/view?usp=sharing) 

<br>
<iframe src ="https://drive.google.com/file/d/1jIQ0Wfs9NheBQGSKlzipJLbvuGi3efoh/preview" width='740' height='430' allowfullscreen mozallowfullscreen webkitallowfullscreen></iframe>
<br>

[Download](https://drive.google.com/file/d/1ZwGIun9K3DtFqcpRCo3hfRYTc5rOS6g1/view?usp=sharing)

### YOLO V4 - Object Detection

In this exercise, we will use a pre-trained network (YOLOv4) to detect objects and people in images. This exercise also teaches how to make a video stream from the computer's camera using google drive, and finally, perform inferences using YOLO V4 from images using the webcam. 

<center>
  <img src="{{ 'assets/img/2022-02-15-computer-vision-basics/od.jpeg' | relative_url }}" width="600" text-align=center alt="img1" />
</center>

[Colab](https://drive.google.com/file/d/1ayBpk8k-qFkne_UGfIBt6EltTfNkjUE0/view?usp=sharing) 

### Retina Face - Face Localization

This exercise shows the results of testing the Retinaface model trained on Tensorflow2.0+. The pre-trained model is downloaded and used in a test image to recognize people's faces and their points of interest. 

<center>
  <img src="{{ 'assets/img/2022-02-15-computer-vision-basics/retinaface.jpeg' | relative_url }}" width="600" text-align=center alt="img1" />
</center>

[Colab](https://drive.google.com/file/d/1MruLLmjDxBDtAZtNEe4giBPB5PBQgXHs/view?usp=sharing) 

### Camera Calibration

This exercise demonstrates how geometric camera calibration estimates the parameters of a lens and image sensor from an image or video. In this notebook, the theory about camera modeling is shown, parameters used, and the transformations necessary to calibrate a camera. From the calibration, it is possible to use the parameters to correct lens distortion, measure the size of an object or determine the location of the camera in the scene. These tasks are used in computer vision applications to detect and measure objects. They are also used in robotics, navigation systems, and 3D scene reconstruction. 

<center>
  <img src="{{ 'assets/img/2022-02-15-computer-vision-basics/cameracalibration.jpeg' | relative_url }}" width="600" text-align=center alt="img1" />
</center>

[Colab](https://drive.google.com/file/d/1q74XroETNmT3-jy1ir1wMBp2HHem1uF1/view?usp=sharing) 

### Fiducial Markers

This exercise shows the use of a resource for estimating poses known as fiducial markers. A fiducial marker is an artificial reference point added to a scene to make it easier to find matching points between images. In this exercise, the theory about the markers and especially about the Aruco marker will be learned. A practical exercise is made showing how to identify and locate these markers in an image. 

<center>
  <img src="{{ 'assets/img/2022-02-15-computer-vision-basics/aruco2.jpeg' | relative_url }}" width="600" text-align=center alt="img1" />
</center>

[Colab](https://drive.google.com/file/d/1_lgW0aeJHUryArxjkNj8fjNVAGQViscs/view?usp=sharing) 


<hr>


<center><h3 class="post-title">Autors</h3><br/></center>
<div class="row">
  <div class=" col-xl-auto offset-xl-0 col-lg-4 offset-lg-0">
    <table class="table-borderless highlight">
      <thead>
        <tr>
          <th><center><img src="{{ 'assets/img/people/diogomartins-1.png' | relative_url }}" width="100" alt="diogo" class="img-fluid rounded-circle" /></center></th>
          <th></th>
          <th><center><img src="{{ 'assets/img/people/israelneto-1.png' | relative_url }}" width="100" alt="israel" class="img-fluid rounded-circle"/></center></th>
          <th></th>
          <th><center><img src="{{ 'assets/img/people/marcoreis8b&w-1.png' | relative_url }}" width="100" alt="marco" class="img-fluid rounded-circle"/></center></th>
        </tr>
      </thead>
      <tbody>
        <tr class="font-weight-bolder" style="text-align: center margin-top: 0">
          <td width="33.33%">Diogo Martins</td>
          <td></td>
          <td width="33.33%">Israel Motta</td>
          <td></td>
          <td width="33.33%">Marco Reis</td>
        </tr>
        <tr style="text-align: center" >
          <td style="vertical-align: top"><small>Robotics Enthusiast. Master student in Mechatronics, Specialist in Robotics and Autonomous Systems, Engineer in Automation and Control. <br> <a href="https://www.linkedin.com/in/diogo-alexandre-martins/">LinkedIn</a></small></td>
          <td></td>
          <td style="vertical-align: top"><small>Research fellow at CC RoSA, Mechatronics Engineer, Specialist in Robotics and Autonomous Systems. <br> <a href="https://www.linkedin.com/in/israel-neto/">LinkedIn</a> </small></td>
          <td></td>
          <td style="vertical-align: top"><small>Senior Researcher - Master in Production Engineering and Electrical Engineer.  <br> <a href="https://www.linkedin.com/in/marco-reis-061618/">LinkedIn</a></small></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
