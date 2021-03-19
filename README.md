1. **create workspace like autonomous_ws **
- cd ~
- mkdir autonomous_ws
- cd autonomous_ws
- mkdir src
- cd src
- git clone git@gitlab.com:emrgry/autonomous_arena.git
- cd ..
- catkin_make

if you already have a workspace;
- cd autonomous_ws/src
- git clone git@gitlab.com:emrgry/autonomous_arena.git
- cd ..
- catkin_make

2. run arena;
- roscore
- create new terminal (ctrl+shift+t)
- cd autonomous_ws
- source devel/setup.bash
- source src/autonomous_arena/setup.sh
- rosrun gazebo_ros gazebo --verbose src/autonomous_arena/worlds/small_track.world
