# TensorRT 端侧部署 + 嵌入式Linux · 学习笔记

## 学习资源
- B站：DeepWok TensorRT部署实战
- B站：正点原子 ARM Linux入门（最新版）
- GitHub：NVIDIA/TensorRT、ultralytics/YOLOv8

## TensorRT 部署

- [ ] PyTorch → ONNX导出
- [ ] TensorRT引擎构建 + FP16/INT8量化
- [ ] 手写前处理、后处理（YOLO的NMS）
- [ ] 端侧性能优化（Batch、Stream、内存复用）
- [ ] YOLOv8/v10部署完整流程

## 嵌入式 Linux

- [ ] Linux常用命令与Shell脚本
- [ ] 交叉编译环境搭建
- [ ] 设备树（DTS）基础修改
- [ ] UART/I2C/SPI驱动控制
- [ ] 嵌入式AI运行环境搭建（Jetson/RK系列）

## 目标
模型在 Jetson/RK3588 上稳定高FPS运行，并打包成ROS2节点
