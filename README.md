# Robotic arm design method
## First we will login to Ubuntu and then we will open Terminal and we will write type those commands:
###
- *Check the dependencies :*

>cd ~/catkin_ws/ 

>catkin_make

>cd ~/catkin_ws/src

>git clone https://github.com/smart-methods/arduino_robot_arm.git 

>cd ~/catkin_ws

>rosdep install --from-paths src --ignore-src -r -y

>sudo apt-get install ros-kinetic-moveit

>sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

>sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

>sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

- *Now we will update your bashrc script with the information about the new workspace:*

>sudo nano ~/.bashrc

- *At the end of the bashrc file we will add the following line:*

>(source /home/wesam/catkin_ws/devel/setup.bash)

- *then ctrl + o*

>source ~/.bashrc

- *The last command to launch the arm:*

>roslaunch robot_arm_pkg check_motors.launch

![image](https://user-images.githubusercontent.com/107880209/181132382-85abd816-10f2-4ca6-b8d1-1eae4e888855.png)
