# Vision-Transformer
## 深度学习课程作业
# Vision Transformer (ViT) for CIFAR-10

这是一个使用 PyTorch 从头开始实现和训练 Vision Transformer (ViT) 的项目，用于 CIFAR-10 图像分类。

## 实验结果

通过精细的结构设计、强数据增强和高级优化策略，本模型在 CIFAR-10 数据集上达到了：

* **验证集峰值准确率:** 85.08%
* **最终测试集准确率:** 85.89%

## 项目结构

```
.
├── models/
│   └── ViT.py         # ViT 模型结构 (PatchEmbedding, TransformerBlock, etc.)
├── utils.py           # 数据加载 (get_data_loaders) 和数据增强 (RandAugment)
├── train.py           # 训练脚本 (带验证)
├── test.py            # 独立的测试脚本
└── requirements.txt   # (可选) 项目依赖
```

## 如何使用

1.  **克隆仓库**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd vit-cifar10-pytorch
    ```

2.  **(可选) 创建环境并安装依赖**
    ```bash
    python -m venv .venv
    source .venv/bin/activate
    pip install torch torchvision timm
    ```

3.  **运行训练**
    ```bash
    python train.py
    ```

4.  **运行测试**
    (训练完成后，将 `test.py` 中的 `MODEL_PATH` 改为你最好的 `.pth` 文件)
    ```bash
    python test.py
    ```
