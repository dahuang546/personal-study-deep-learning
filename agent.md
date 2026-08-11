# Agent Instructions

## 对话总结
每次对话结束时，自动总结本次内容并记录到这里。

## 项目信息
- 用途：深度学习学习代码
- 目录：`G:/学习课件/2026/8/nnlearn`
- 文件：
  - `micograd.ipynb`：自动微分 `Value` 类实现（micrograd 风格），含加/乘/tanh/反向传播与 graphviz 可视化
  - `neuron-net.ipynb`：当前为空
- GitHub 用户名：dahuang546
- GitHub 仓库名：personal-study-deep-learning
- GitHub 仓库地址：https://github.com/dahuang546/personal-study-deep-learning.git
- GitHub 认证方式：SSH（已通过认证）

## 待办
- [x] 完成 GitHub 认证
- [x] 创建/指定 GitHub 仓库
- [x] 初始化 git 并推送文件

## 对话总结（2026-08-07）
本次完成了 GitHub 上传前的全部初始化工作：
1. 在 `~/.ssh/` 下生成了 ed25519 SSH 密钥，并将公钥添加到 GitHub；
2. 测试 SSH 连接成功，GitHub 用户名为 `dahuang546`；
3. 本地执行了 `git init`，添加 `.gitignore` 排除 `.venv/`、`__pycache__/`、`.ipynb_checkpoints/`；
4. 提交了 `2.ipynb`、`3.ipynb`、`agent.md`、`.gitignore`；
5. 推送到远程仓库 `git@github.com:dahuang546/personal-study-deep-learning.git`，分支为 `main`。

仓库地址：https://github.com/dahuang546/personal-study-deep-learning

## 对话总结（2026-08-08）
1. 检查 `2.ipynb` 中 `Value` 类的反向传播实现：
   - 确认 `+`、`*`、`tanh` 的局部 `_backward` 实现正确，`+=` 累加 grad 可处理节点复用；
   - 指出缺少**自动反向传播**（缺少按拓扑排序调用所有 `_backward` 的通用方法），用户表示这是故意留的练习；
   - 指出 `other` 暂不支持普通数字（如 `a * 2`），建议后续需要时再补转换逻辑。
2. 创建 `log.md` 作为推送日志，记录每次推送到 GitHub 的内容简介。
3. 将 `2.ipynb` 和 `log.md` 推送到远程仓库，提交为 `ad28e68`。

## 注意事项
- SSH 密钥保存在 `~/.ssh/id_ed25519.pub`（公钥）和 `~/.ssh/id_ed25519`（私钥），**私钥不要外泄**；
- 推送到 GitHub 时请使用 SSH 地址：`git@github.com:dahuang546/personal-study-deep-learning.git`，不要搞成 HTTPS；
- `3.ipynb` 当前被忽略，不推送到 GitHub，等里面有内容后再决定。
- 每次推送时记得在 `log.md` 追加一条内容简介记录。
