# Enterprise AI Value Explorer · 企业 AI 投入与价值交互图

一个可以直接运行的交互演示：让项目负责人通过曲线讨论 **自建 FDE 团队成本、项目投入、产能价值与安全情景**，同时阅读背后的业务解释。

Interactive scenario explorer for enterprise AI investment, delivery costs and capacity value. The defaults are illustrative assumptions, not measured ROI or cash profit.

**[在线试用](https://fanh6591-ux.github.io/enterprise-ai-value-explorer/) · [原官网版本](https://isaac2024.online/enterprise-faq/) · [企业 AI 项目指南](https://github.com/fanh6591-ux/enterprise-ai-playbook)**

![模型静态预览](docs/preview.svg)

*预览由模型直接生成，在线演示可操作；图中数字均为假设。*

## 30 秒开始

下载仓库后直接打开 `index.html`；也可运行：

```bash
git clone https://github.com/fanh6591-ux/enterprise-ai-value-explorer.git
cd enterprise-ai-value-explorer
python3 -m http.server 8968 --bind 127.0.0.1
```

打开 http://127.0.0.1:8968 。所有脚本和图表依赖已包含，可离线运行，无需账户、模型服务、API 密钥或安装包。

## 试试这三个动作

1. 拖动或缩放图表，观察不同投入时点与后续范围。
2. 点“自建 FDE 成本”“累计总投入”或“产能价值”，阅读与曲线对应的说明。
3. 开启安全事故情景，再恢复正常推演，观察假设如何改变图形。

## 怎样修改

| 文件 | 修改内容 |
|---|---|
| `model.js` | 数值假设、计算与图表选项；从 `defaults` 开始 |
| `stories.js` | 曲线对应的说明、阅读片段与来源 |
| `explorer.js` | 交互、推演、缩放与无障碍状态 |
| `explorer.css` | 图表与阅读布局 |
| `index.html` | 独立演示入口 |

默认数字是情景示例；不是市场报价、已验收客户业绩或事故概率。产能价值需要实际利用才可能转化为现金结果，不能直接当作利润。自建团队和外部交付是不同选择，不应重复相加。

迁出官网时为独立页面补了标题、使用入口与口径说明，并将摘要中的“利润”改为“价值差额”；原有模型计算没有更改。官网版本保持原样。来源与文件摘要见 `source-manifest.json`。

## 欢迎贡献

适合贡献的问题：读图是否清楚、手机操作是否顺手、假设口径是否明确，以及可复现的计算错误。请在 Issue 中写出操作步骤、预期结果与实际结果。讨论真实客户场景时请使用匿名或合成资料。

未来可以增加假设导入导出、可核对的试点记录和英文说明；这些尚未实现。当前页面用于方法交流和情景讨论。

## 许可

本站拆出的模型、交互、样式、说明与独立入口采用 MIT 许可。Apache ECharts 6.0.0 保留 Apache-2.0 许可及完整 LICENSE/NOTICE，见 `vendor/`。

维护者：[何凡 Isaac](https://github.com/fanh6591-ux) · [企业 AI 咨询与共创](https://isaac2024.online/#contact)
