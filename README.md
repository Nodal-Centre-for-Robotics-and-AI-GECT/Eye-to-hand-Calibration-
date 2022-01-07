# Eye-to-hand-Calibration-
Eye to hand calibration of Aubo i5 robot and Kinect v2

eye to  hand Calibration

This is a package to perform the  eye to hand  calibration to get the transformation between the robot base link  and camera  . Here we used aubo_15 robot and intelrealsense Kinect v2  depth camera. Here we use a aruco marker (100 ) as the calibration image and aruco_hand_eye as calibration package
1. Development Environment

    Ubuntu 16.04.2
    ROS Kinetic

2. ROS Package Dependencies

    aubo_robot  ( https://github.com/Nodal-Centre-for-Robotics-and-AI-GECT/aubo_i5_pick-and-place)
    kinect2_bridge (https://github.com/code-iai/iai_kinect2)
    visp_hand2eye_calibration (http://wiki.ros.org/visp_hand2eye_calibration)
    aruco_ros    (http://wiki.ros.org/aruco_ros)
    aruco_hand_eye ( https://github.com/jhu-lcsr/aruco_hand_eye)

Step 1: Install the dependencies

Step 2: Experiment setup

attach the camera to the base link  of the robot

Step 3: inster test.launch in the launch folder of aruco_hand_eye package
Bring up the camera and robot
by lauching test.launch in aruco_hand_eye package
step 4: 
rosrun visp_hand2eye_calibration visp_hand2eye_calibration_client
rosrun visp_hand2eye_calibration visp_hand2eye_calibration_calibrator

Then run  hand_eye.py  
move the arm and follow procedure prompts
