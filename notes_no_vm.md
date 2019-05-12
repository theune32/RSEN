# Doing the Robotics Software Engineer Nanodegree from a linux machine (no VM or workspace)

## Characteristics
- Ubuntu 18.04.2 LTS
- ROS version Meldocic(!)
- Gazebo version ?

## Tips
Always run `sudo apt-get update && sudo apt-get upgrade -y`
I can recommend Visual Studio Code, easily used for multiple programming and scripting languages in the same project/folder.
For using multiple terminals I can recommend tmux, it is very easy to create multiple windows and split them. And then have hotkeys to move between them!

## Errors handled/solved/worked around
- Gazebo giving error:
  `[Err] [REST.cc:205] Error in REST request`
  Solution described [here](https://bitbucket.org/osrf/gazebo/issues/2607/error-restcc-205-during-startup-gazebo)
- Gazebo bug/missing functionality:
    Interesting find, you cannot edit existing/saved buildings. Some aspects are changeable but not much.
- Multiple errors having to do with controllers not being able to be found.
    In the end I ended up installing/updating some ros melodic packages:
    ```sudo apt-get install ros-melodic-ros-control ros-melodic-ros-controllers ros-melodic-joint-state-controllers```
