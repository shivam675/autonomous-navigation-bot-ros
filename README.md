# autonomous-navigation-leo

Major Dependencies: ros-melodic-desktop-full
              python2

This ros -melodic version package contains gazebo simulator launch files for launching a custom world file and leo rover in it.

1. Start with cloning the repo into src of catkin workspace
2. Run following lines in terminal in catkin_ws where you have your src folder
'''
rosdep install --from-paths src --ignore-src --rosdistro=melodic -y
'''
'''
catkin_make
'''
'''
source devel/setup.bash
'''
3. Start with
'''
roslaunch robot_gazebo main_indoor_with_person.launch
'''
'''
then,
roslaunch robot_gazebo final.launch
'''
'''
roslaunch leo_nav nav.launch
'''

Check the things in gazebo and rviz and confirm there are no errors.
Add things by topic in gazebo and then give correct 2d pose of the bot
then give a 2d goal to the bot. If all goes fine the bot should start moving towards goal.
