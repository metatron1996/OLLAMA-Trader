# OLLAMA-Trader: AI 自主进化量化交易平台

OLLAMA-Trader 是一个集成了大型语言模型 (LLM) 的高级量化交易平台，具备**自主学习**和**自我进化**的能力。它不仅仅是一个交易机器人，更是一个能够随着市场变化而不断优化自身的智能交易生态系统。

## ⚠️ 注意事项

> **！！这个世界上没有百分百赚钱的方法！！**
> 
> **！！请谨慎投资，见好就收，切勿存在赌徒心理！！**
> 
> **！！请谨慎投资，见好就收，切勿存在赌徒心理！！**
> 
> **！！请谨慎投资，见好就收，切勿存在赌徒心理！！**

## 核心功能

*   🧠 **AI 自主进化**:
    *   **代码优化**: 自动分析和重构性能瓶颈，提升算法效率。
    *   **Prompt 优化**: 持续优化与 LLM 的交互，以提高决策的准确性。
    *   **架构感知**: 能够识别系统级的潜在问题并提出改进建议。

*   📈 **自主学习与策略生成**:
    *   **经验驱动**: 从每一笔交易中学习，无论是成功还是失败。
    *   **模式发现**: 自动识别新的市场模式和交易机会。
    *   **动态规则库**: AI 可以直接修改和完善自身的交易规则和策略。

*   🤖 **OLLAMA 集成**:
    *   利用本地运行的 LLM (如 Llama 3, Qwen 2.5) 进行复杂的市场分析和交易决策。
    *   支持通过 OLLAMA 进行自然语言交互，分析市场情绪。

*   📊 **全面的交易与分析工具**:
    *   **多交易所支持**: 已集成 Binance 和 OKX。
    *   **高级图表**: 提供丰富的可视化工具，用于市场分析和策略回测。
    *   **风险管理**: 内置订单守卫、追踪止损和持仓巡检等功能。
    *   **巨鲸监控**: 实时监控大额交易，洞察市场动向。

*   🖥️ **用户友好的图形界面**:
    *   基于 PySide (Qt) 构建的现代化、响应迅速的交易中心。
    *   ## 软件工作原理

本系统的工作流程可以概括为以下几个步骤：

1.  **数据收集**: 系统从交易所 (Binance, OKX) 实时获取市场数据，包括 K 线、深度和成交量。
2.  **AI 分析与决策**:
    *   收集到的数据被送入 OLLAMA 进行分析。
    *   OLLAMA 根据其内部知识库中的规则和策略，结合当前市场情况，做出“买入”、“卖出”或“持有”的决策。
3.  **执行与监控**: 
    *   如果 AI 决定进行交易，系统会自动执行订单。
    *   “订单守卫”模块会持续监控订单状态，确保其顺利执行。
4.  **经验记录**: 每一笔交易，无论盈亏，都会被详细记录在“实盘经验库”中。
5.  **自主学习与进化**: 
    *   在系统空闲时，AI 会自动分析经验库中的数据。
    *   它会从中总结成功和失败的模式，并利用这些洞察来更新和优化其知识库中的交易规则和策略。
    *   在“自我进化”模式下，AI 甚至可以修改自身的代码，以提高运行效率或修复潜在的 bug。

这个闭环的学习和进化过程，使得系统能够不断适应变化的市场，并持续提升其交易表现。

## 技术栈

*   **后端**: Python
*   **数据科学**: Pandas, NumPy, SciPy
*   **机器学习**: TensorFlow, PyTorch, Scikit-learn, XGBoost
*   **GUI**: PySide (Qt for Python)
*   **Web 框架**: FastAPI, Streamlit
*   **交易所接口**: CCXT, python-binance
*   **数据库**: SQLite
*   **可视化**: Matplotlib, Plotly, Seaborn

## 系统架构

OLLAMA-Trader 采用模块化架构，主要包括以下几个核心组件：

1.  **交易中心 (Trading Center)**: 基于 Qt 的主应用程序，是用户与系统交互的入口。
2.  **功能模块 (Functional Modules)**:
    *   `ai`: 包含了所有与 AI 相关的功能，如 OLLAMA 集成、自主学习和自我进化。
    *   `intel`: 用于情报收集，如巨鲸监控。
    *   `utils`: 提供各种工具函数。
3.  **数据中心 (Data Hub)**: 负责数据的获取、存储和管理，包括市场数据、交易记录和学习成果。
4.  **知识库 (Knowledge Base)**: 存储由 AI 自主学习和优化的交易规则、策略和模式。
5.  **脚本 (Scripts)**: ## 快速开始

1.  **克隆仓库**:
    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2.  **安装依赖**:
    建议在虚拟环境中使用 Python 3.11 或更高版本。
    ```bash
    pip install -r requirements.txt
    ```

3.  **配置 OLLAMA**:
    确保你已经在本地安装并运行了 OLLAMA。你可以从 [ollama.com](https://ollama.com) 下载。

4.  **配置 API 密钥**:
    在 设置中可以直接绑定并激活交易所API_Key
5.  **运行程序**:
    ```bash
    run_qt_app.cmd
    /
    python run_qt_app.py
    ```

## 使用指南

### AI 托管模式

在 AI 托管模式下，系统将利用 OLLAMA 和其内部知识库来自动进行交易决策。你可以实时监控 AI 的行为、决策过程和性能指标。

### 自主学习

系统会在空闲时自动触发自主学习过程。你可以在“学习”选项卡中查看学习日志、新发现的模式以及对交易规则的调整。

### 自我进化

## 配置

主要的配置文件位于 `config/` 目录下：

*   `default_config.json`: 主配置文件，包含交易参数、AI 配置等。
*   `logging_config.json`: 日志系统配置。
*   `rules_config.json`: 初始的交易规则配置。

## 开发

我们欢迎社区的贡献！如果你希望为 OLLAMA-Trader 做出贡献，请遵循以下步骤：

1.  Fork 本仓库。
2.  创建一个新的分支 (`git checkout -b feature/your-feature`)。
3.  提交你的修改 (`git commit -m 'Add some feature'`)。
4.  推送到你的分支 (`git push origin feature/your-feature`)。
5.  创建一个新的 Pull Request。

## 许可证

本项目采用 [MIT 许可证](LICENSE)。

## 联系方式

如果你有任何问题或建议，请通过以下方式联系我们：

*   **GitHub Issues**: [https://github.com/your-username/your-repo/issues](https://github.com/your-username/your-repo/issues)
## 打赏

如果这个项目对你有帮助，欢迎通过以下方式支持我的开发工作：

**TRC20 地址**: `TD6dXAxPMRR84KuviyVivAsyovUK95s7NJ`

<img width="302" height="352" alt="image" src="https://github.com/user-attachments/assets/3c81cf48-f7f3-4a1d-903a-749c42a9fdd4" />

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/2f8b10bf-c458-4d72-9b08-3d7cab071b90" />

<img width="1000" height="600" alt="image" src="https://github.com/user-attachments/assets/4e29a814-9b85-49b7-8ca0-cb7aa5b3ed61" />

<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/c97a00de-5449-45f3-a08e-99d36d4e0c09" />

<img width="1920" height="1009" alt="image" src="https://github.com/user-attachments/assets/f049173a-1b99-4416-9daf-a8c3d116ab24" />

<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/2d61c5c5-a4a1-420f-97e7-53d5f1870b97" />





