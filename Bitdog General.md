# Bitdog General  
## How to ssh into Go1  
[How to connect to Go1](/How%20to%20connect%20to%20Go1.md)  
  
## How to start Lidar RVIZ  
  
adapted from https://yesandy.github.io/posts/go1-doc2/  
- Connect to Go1 using an ethernet cable.  
- Check if you are in the subnet 192.168.123.42/24 ([How to change subnet](/How%20to%20change%20subnet.md))  
- `export ROS_MASTER_URI=http://192.168.123.15:11311` on the local machine and on the NVIDIA Jetson  
- `export ROS_IP=192.168.123.15??????` Unsure how this works or if it even does anything  
#### Starting the lidar on Jetson  
```bash  
cd UnitreeSLAM/catkin_slam_3d  
source devel/setup.bash  
roslaunch start build_map.launch map_name:=your_map_name  
```  
#### Starting rviz  
```bash  
rosrun rviz rviz -d buildmap.rviz  
```  
buildmap.rviz is some kind of package/configuration file for rviz offered by catkin_3d itself  
  
#### Bitdog's wifi and PI stopped working  
[We got go1's internet working somehow](/We%20got%20go1's%20internet%20working%20somehow.md)