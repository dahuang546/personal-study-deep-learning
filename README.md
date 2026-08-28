# personal-study-deep-learning

个人深度学习学习记录仓库。

这里主要用来放自己学习深度学习过程中写的代码、笔记和实验，方便随时回顾和整理。
> 目前处于随手记录阶段，内容会随学习进度慢慢补充。

## 环境信息

本仓库使用 `.venv/` 下的本地虚拟环境，主要信息如下：

- Python 版本：3.13.3
- PyTorch：`2.13.0+cpu`（CPU 版本，无 GPU）
- 主要依赖：`numpy` 2.5.1、`pandas` 3.0.5、`matplotlib` 3.11.1、`scikit-learn` 1.9.0、`scipy` 1.18.0、`jupyterlab` 4.6.2、`notebook` 7.6.1、`torchvision` 0.28.0+cpu、`torchaudio` 2.11.0+cpu、`graphviz` 0.21
- 完整 `pip list` 见 [requirements.txt](./requirements.txt)


## 仓库结构

- `micograd/`：micrograd 学习代码
  - `micograd.ipynb`：自动微分 `Value` 类实现（micrograd 风格）
  - `log.md`：micograd 部分的提交与修改记录
  - `README.md`：文件夹说明
- `makemore/`：makemore 系列学习代码
  - `bigram-ENGLISH/bigram-ENGLISH.ipynb`：英文 bigram 名字生成模型
  - `bigram-CHINESE/bigram-CHINESE.ipynb`：中文 bigram 名字生成模型（**新增**，待实现）
  - `log.md`：makemore 部分的学习日志与提交记录
  - `README.md`：文件夹说明
- `neuron-net.ipynb`：当前为空，后续用于神经网络相关实验（暂不推送到 GitHub）
