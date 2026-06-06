# 🔵🟢 AI Blue-Green Tools

AI蓝绿部署工具，支持蓝绿部署、金丝雀发布、滚动更新。

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python" />
  <img src="https://img.shields.io/badge/OpenAI-API-green?logo=openai" />
  <img src="https://img.shields.io/badge/License-MIT-yellow" />
</p>

## ✨ 特性

- 🔵🟢 蓝绿部署设计
- 🐦 金丝雀发布设计
- ☸️ K8s Rollout配置
- 🔄 流量分割设计
- 🔷 Istio VirtualService
- 🔄 回滚策略设计

## 🚀 快速开始

```bash
pip install openai

python tools.py
```

## 📖 使用

```python
from ai_blue_green_tools import create_tools

tools = create_tools()

# 蓝绿部署
bg = tools.design_blue_green("API服务", {"zero_downtime": True})

# 金丝雀发布
canary = tools.design_canary_release("API服务", stages)

# K8s Rollout
rollout = tools.generate_k8s_rollout("API服务", "金丝雀")

# 流量分割
traffic = tools.design_traffic_splitting("API服务", ["Header", "Cookie"])

# Istio VirtualService
istio = tools.generate_istio_virtual_service("API服务", ["api.example.com"])

# 回滚策略
rollback = tools.design_rollback_strategy("API服务", ["错误率>5%"])
```

## 📁 项目结构

```
ai-blue-green-tools/
├── tools.py       # 蓝绿部署工具核心
└── README.md
```

## 📄 许可证

MIT License
