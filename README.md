# 剔除评论分析

基于pytorch，采用bert-base-chinese预训练模型做评论分类，分为0,keep;1,remove两个类别。

为改进样本数量不均匀的问题，损失函数采用FocalLoss。经测试，训练模型在训练集上的预测准确度：99.8618%；在测试集上的预测准确度：99.0890%。

## 文件结构

| 文件名                 | 功能     |
| :--------------------- | -------- |
| **train.py**           | 模型训练 |
| **data_process.py**    | 生成数据 |
| **inference.py**       | 快速测试 |
| **iTrainingLogger.py** | 绘图     |

## 运行
```
python train.py
```
