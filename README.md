# Yoga Pose Detection (PoseNet)

This project utilizes computer vision and machine learning techniques to detect and classify yoga poses in real-time using a webcam. It provides an interactive and visual way for yoga practitioners to receive real-time feedback on their poses.

## Features

- Real-time pose detection and classification using computer vision techniques
- Supports multiple yoga poses, including Downward Dog, Warrior Pose, Tree Pose, etc.
- Webcam integration for capturing live video
- Visual feedback on the detected pose, including key body joints and angles
- Pose classification accuracy and confidence level display

## Basic Theory

Yoga pose estimation is the detection and recognition of specific yoga poses performed by a person using computer vision techniques. Practising yoga can improve flexibility, strength, and overall physical fitness, while also promoting relaxation and reducing stress levels. The goal of the project is to help common people practice yoga poses with proper posture and body alignment on their own, in order to prevent serious injuries that can be caused by practising yoga asanas with incorrect body alignment in the long run. Getting feedback on the correctness of the yoga posture can have huge benefits in learning and practising the yoga asanas. The project is an implementation of OpenCV and Mediapipe libraries. OpenCV is an open-source computer vision library that provides a wide range of functions for image and video processing. MediaPipe is a cross-platform, high-fidelity body pose tracking solution framework, that is used for building multi-modal applied machine learning pipelines. The project utilises MediaPipe to obtain the 33 major landmark coordinates of the human body. MediaPipe utilizes BlazePose[1] topology, a superset of COCO[2], BlazeFace[3], and BlazePalm[4] topology. These landmark coordinates form the basis for the pose estimation. The appropriate angles formed by landmarks while performing the asana precisely are compared to the person’s live feed of performingthe asana. The project then provides voice feedback so that the person can make alterations to the pose and avoid misalignment of the body so that the yoga asana can be performed efficiently without developing aches while attaining the numerous benefits of practising yoga.
So,Using PoseNet we get key points of human limbs. Output of keypoints is (x,y) co-ordinate value. Then using these keypoints we can determine angles of different limb of our body or can use these point in classifier model for human acitivity detection. There are some out performing model for pose estimation like: OpenPose pose estimation model which can also be inferenced in CPU.


## Running
```python main.py runserver```


## DataSet
[Data](https://drive.google.com/file/d/1n5qpMEGmW_-urhTatfRecva8dHQMTgdK/view?usp=sharing)

## Training

I prepared the training procedure using UI. By clicking the button we can select current frame considering this as level. Open ```index.html``` in editor from training folder, some thing will apear like below


## Output

<p align="center">
  <img width="600" height="500" src="https://github.com/Trisha3620/Yoga_pose_Detection/blob/main/Final.png">
</p>
