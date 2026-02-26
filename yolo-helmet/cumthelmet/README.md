# 数据集结构说明

此数据集包含以下类别:
helmet, no-helmet

数据集划分:
- 训练集: 80%
- 验证集: 10%
- 测试集: 10%

目录结构:
D:\dataset\CUMT-HelmeT\dataset/
├── train/
│   ├── images/     # 训练集图像
│   └── labels/     # 训练集标签
├── val/
│   ├── images/     # 验证集图像
│   └── labels/     # 验证集标签
├── test/
│   ├── images/     # 测试集图像
│   └── labels/     # 测试集标签
├── no_target/      # 不含目标类别的图像
├── classes.names   # 类别名称文件
└── data.yaml       # YOLO 配置文件

使用说明:
1. 使用 data.yaml 文件配置 YOLO 训练
2. 训练命令示例: yolo train data=data.yaml model=yolov8n.pt
