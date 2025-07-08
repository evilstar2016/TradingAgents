# 项目结构与功能说明

```
LICENSE                  # 开源协议文件
main.py                  # 项目主入口，启动和调度核心逻辑
pyproject.toml           # Python项目配置文件
README.md                # 项目说明文档
requirements.txt         # Python依赖列表
setup.py                 # 安装脚本
uv.lock                  # 依赖锁定文件
assets                   # 项目图片资源目录
├── analyst.png          # 分析师头像
├── researcher.png       # 研究员头像
├── risk.png             # 风控头像
├── schema.png           # 系统结构图
├── TauricResearch.png   # 品牌Logo
├── trader.png           # 交易员头像
├── wechat.png           # 微信二维码
└── cli                  # CLI界面相关图片
    ├── cli_init.png
    ├── cli_news.png
    ├── cli_technical.png
    └── cli_transaction.png
cli                      # 命令行交互模块
├── __init__.py          # 包初始化
├── main.py              # CLI主入口，用户交互、界面布局
├── models.py            # CLI相关数据模型（如分析师类型）
├── utils.py             # CLI工具函数（如分析师选择、日期选择等）
└── static
    └── welcome.txt      # CLI欢迎信息

doc                      # 文档目录
└── project_overview.md  # 项目结构与说明（本文件）

tradingagents            # 核心功能包
├── default_config.py    # 默认配置项
├── agents               # 智能体相关模块
│   ├── __init__.py      # 包初始化
│   ├── analysts         # 各类分析师
│   │   ├── fundamentals_analyst.py    # 基本面分析师
│   │   ├── market_analyst.py          # 市场分析师
│   │   ├── news_analyst.py            # 新闻分析师
│   │   └── social_media_analyst.py    # 社交媒体分析师
│   ├── managers         # 管理者
│   │   ├── research_manager.py        # 研究管理者
│   │   └── risk_manager.py            # 风控管理者
│   ├── researchers      # 研究员
│   │   ├── bear_researcher.py         # 空头研究员
│   │   └── bull_researcher.py         # 多头研究员
│   ├── risk_mgmt        # 风控辩手
│   │   ├── aggresive_debator.py       # 激进辩手
│   │   ├── conservative_debator.py    # 保守辩手
│   │   └── neutral_debator.py         # 中性辩手
│   ├── trader           # 交易员
│   │   └── trader.py                  # 交易员实现
│   └── utils            # 智能体工具
│       ├── agent_states.py            # 智能体状态定义
│       ├── agent_utils.py             # 智能体通用工具
│       └── memory.py                  # 智能体记忆体
├── dataflows            # 数据流与外部数据源
│   ├── __init__.py      # 包初始化
│   ├── config.py        # 数据流配置
│   ├── finnhub_utils.py # finnhub数据接口
│   ├── googlenews_utils.py            # Google新闻接口
│   ├── interface.py     # 统一数据接口
│   ├── reddit_utils.py  # Reddit数据接口
│   ├── stockstats_utils.py            # 技术指标工具
│   ├── utils.py         # 通用工具
│   └── yfin_utils.py    # 雅虎财经数据接口
└── graph                # 智能体图结构与信号处理
    ├── __init__.py      # 包初始化
    ├── conditional_logic.py           # 条件逻辑
    ├── propagation.py   # 信号传播
    ├── reflection.py    # 反射机制
    ├── setup.py         # 图结构初始化
    ├── signal_processing.py           # 信号处理
    └── trading_graph.py # 交易智能体图
```

> 本文档由自动化工具生成，涵盖各目录、子目录及主要文件的树形结构和功能说明，便于快速了解项目结构。
