# ROS2 工作空间

## 环境要求
- Ubuntu 22.04
- ROS2 Humble

## 构建

```bash
cd ros2_ws
colcon build
source install/setup.bash
```

## 功能包规划

```
ros2_ws/src/
├── my_first_pkg/          # 入门练习（Topic/Service/Action）
├── camera_pkg/            # 相机图像处理（CvBridge）
├── yolo_detect_pkg/       # YOLO检测ROS2节点
└── agent_bridge_pkg/      # Agent指令桥接节点
```
