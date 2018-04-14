# dlive-navigation
This repository includes the config and yaml files for the ROS Navigation Stack, implemented on our driverless car. 

We use the teb_local_planner(http://wiki.ros.org/teb_local_planner) as a local planner for the car.

We are using the rtabmap_ros(http://wiki.ros.org/rtabmap_ros/Tutorials/StereoOutdoorNavigation) with our zed_stereo camera(https://www.stereolabs.com/)for doing the Simulataneous Localisation and Mapping.

The point clouds created by rtabmap are used by the ROS Navigation Stack for calculating a collision-free path.

In the future, we also plan to include a custom costmap layer for Segnet(http://mi.eng.cam.ac.uk/projects/segnet/) which we use for road detection.

To run ROS Navigation on the car, do a:
    
      roslaunch dlive-navigation car_stereo_nav.launch
