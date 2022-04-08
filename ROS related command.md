## rostopic related command
```bash
rostopic list #list all current running ros topic
rostopic info ${topic_name} # show the information of the ${topic_name}
rostopic echo ${topic_name} # show the output of the ${topic_name} 
```
    
## show PCD file through pcl
```bash
rosrun pcl_ros pcd_to_pointcloud ${file.pcd}
```
    
## 杀死已关闭ssh的roscore
```bash
killall -9 rosmaster
```
    
## rospkg not found in conda
```bash
pip3 install rospkg
```
