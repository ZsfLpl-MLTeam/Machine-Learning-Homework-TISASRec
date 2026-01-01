# Machine-Learning-Homework-TiSASRec

Here's the machine learning project repository for **zsf** and **lpl** at **Sun Yat-sen University**.

## 模型介绍与使用说明

本项目包含两个基于 TiSASRec 的改进版本，请参考以下说明进行部署和运行。

### 1. TiSASRec-R (消融实验版)

* **文件名称**: `TiSASRec-R.py`
* **模型简介**: 该模型是依照原论文中**消融实验 (Ablation Study)** 的思路改进而成的 TiSASRec-R 版本。
* **使用方法**:
    1.  请将该文件移动至ReChorus项目的 `src/models/sequential` 目录下。
    2.  在运行测试命令时，将 `--model_name` 参数修改为以下内容即可运行：
        ```bash
        --model_name TiSASRec_R
        ```

### 2. TiSASRecPlus (对数尺度改进版)

* **文件名称**: `TiSASRecPlus.py`
* **模型简介**: 该模型在原 TiSASRec 的基础上进行了改进，引入了**对数尺度连续时间编码 (Log-Scale Continuous Time Encoding)** 机制，以提升在不同密度数据集上的表现。
* **使用方法**:
    1.  请将该文件移动至ReChorus项目的 `src/models/sequential` 目录下。
    2.  在运行测试命令时，将 `--model_name` 参数修改为以下内容即可运行：
        ```bash
        --model_name TiSASRecPlus
        ```
