# Push Log

记录每次推送到 GitHub 的内容简介。

## 2026-08-08

- 更新 `2.ipynb`：添加 `Value` 类反向传播基础实现，包含 `+`、`*`、`tanh` 操作的局部 `_backward`，以及 graphviz 计算图可视化。
- 更新 `agent.md`：记录代码检查反馈、创建 `log.md` 及本次推送操作。

## 2026-08-08

- 修复 `2.ipynb` 中 `Value` 类反向传播命名冲突：将局部梯度函数改名为 `_backward`，保留公共方法 `backward()`，实现基于拓扑排序的自动反向传播。
- 现在调用输出节点的 `backward()` 即可自动完成全图梯度回传，无需再手动链式调用每个中间节点。

## 2026-08-09

- 大幅扩展 `2.ipynb`：为 `Value` 类补充大量基础运算，完善整体框架。
- 包含 `exp`、`log`、`pow`、`div`、`neg`、`sub`、`relu` 等新增操作及对应的反向传播实现。
- 奠定了后续构建更复杂神经网络的基础。
- 现在调用输出节点的 `backward()` 即可自动完成全图梯度回传，无需再手动链式调用每个中间节点。

## 2026-08-11

- 文件重命名：`2.ipynb` → `micograd.ipynb`，`3.ipynb` → `neuron-net.ipynb`。
- 同步更新 `.gitignore` 与 `agent.md` 中的文件说明。
- `neuron-net.ipynb` 仍被忽略，暂不推送到 GitHub。
