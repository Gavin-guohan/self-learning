# TensorRT 端侧部署代码

## 环境要求
- CUDA 11.x / 12.x
- TensorRT 8.x+
- PyTorch (导出用)
- ONNX Runtime (验证用)

## 目录结构

```
tensorrt_deploy/
├── export/                # PyTorch → ONNX 导出脚本
├── build_engine/          # ONNX → TensorRT 引擎构建
├── inference/             # TensorRT 推理代码
├── preprocess/            # 手写前处理
├── postprocess/           # 手写后处理（NMS等）
└── benchmark/             # 性能测试脚本
```
