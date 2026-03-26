# Gemini CLI 扩展：公式逆向工程 (Formula Reverse Engineering)

这是一个专为 [Gemini CLI](https://github.com/google/gemini-cli) 设计的专业扩展，旨在将你的 AI Agent 转化为一名资深数据科学家，使其具备从多维黑盒数据中还原复杂评分算法和数学模型的能力。

## 🌟 核心理念

与其让 AI 盲目地用随机多项式或神经网络去拟合数据，本扩展强制执行一套严谨的 **7 步迭代方法论**。这种方法特别适用于分析人类设计的系统（如金融评分、物理模型、业务指标），因为它优先追求**“物理优雅性”**——即寻找人类设计者原本意图使用的简洁整数、比例和标准函数。

## 🛠 7 步迭代方法论

1.  **探索性拟合 (Exploratory Fitting)**：快速测试各维度的相关性，建立初步理解。
2.  **隔离与锁定 (Isolate & Control)**：一旦确认某个变量的线性关系，立即锁定参数并将其剔除，以降低剩余问题的维度。
3.  **离群值分析 (Outlier Analysis)**：专门针对残差最大的点，寻找公式中缺失的变量或逻辑漏洞。
4.  **切片与分段 (Slicing & Segmentation)**：通过窄频切片或 0 值切片，重建真实的阈值（Floor/Ceiling）和逻辑分支。
5.  **多项式探测与形状猜想 (Shape Guessing)**：利用高阶多项式描绘曲线几何形状，反推底层的解析表达式（如 Log, Exp, Arcsinh）。
6.  **融合 (Fusion)**：将零散的分段逻辑重新整合成高维度的统一数学规律。
7.  **物理优雅化 (Physical Elegance)**：消除丑陋的机器生成小数，将系数强制对齐到人类直觉中的整数或简洁分数。

## 📦 安装

直接通过 Gemini CLI 安装：

```bash
gemini ext install https://github.com/roshameow/gemini-ext-reverse-engineering
```

然后在交互模式下重新加载 skills：
```text
/skills reload
```

## 💡 使用示例

只需要求 Gemini CLI 分析你的数据集并寻找底层公式。Agent 将自动触发该 skill 并严格遵循 7 步专家工作流。

*示例提示词：*
- “这里有一组包含 Sharpe, Turnover, Returns, 和 Drawdowns 映射到评分 Score 的数据。请帮我逆向出底层的评分公式。”
- “我有一组黑盒物理实验数据。请使用 `formula-reverse-engineering` skill 帮我找出其背后优雅的数学方程。”

## 📄 许可证

MIT License
