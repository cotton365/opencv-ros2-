# opencv-ros2-  还有循迹小车
1.基于ROS2 OPENCV的一个识别蓝色 红色的程序
程序就是这个py代码  
其实代码也是2个月前的代码，现在和小车的整合  
2.小车代码在rar文件里  
3.在ros2这个程序构建上，整合好后这样执行  
重新构建
cd ~/ros2_ws
colcon build --packages-select camera_processing
source install/setup.bash

运行摄像头节点（使用HSV方法）
ros2 run camera_processing camera_node

运行图像处理节点（使用RGB方法）
ros2 run camera_processing image_processor_node
