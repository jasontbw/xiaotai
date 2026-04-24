# SKILLS_MANIFEST.md - 详情页助手技能清单与流水线

配置完成时间：2026-04-24
状态：已锁定，不再变动

---

## 📦 已安装技能清单（7 个核心技能）

| # | 技能名称 | 版本/来源 | 核心能力 |
|---|----------|-----------|----------|
| 1 | **markdown-new-crawl** | clawhub/ctxinf | ✅ 带链接递归解析的 Markdown 数据精准抽取，能打开文档中的超链接和子文档抓取全文 |
| 2 | **seo-geo-playbook** | clawhub/gingiris | ✅ 英文 GEO 长文案与 FAQ 生成，按固定栏目输出，专业且有销售力 |
| 3 | **deep-search** | clawhub/aiwithabidi | ✅ 大模型网络深度搜索与事实整合，基于已有信息生成搜索摘要并检索英文网络 |
| 4 | **huoshan-ai-generator** | 本地内置 | ✅ 火山引擎 SeaDream 5.0 Lite 图片生成，写实风格工业品配图 |
| 5 | **html-analysis** | clawhub/mzlzyca | ✅ 网页结构与配色学习，能学习参考页面的 DOM 结构、配色、字体、按钮样式 |
| 6 | **schema-gen** | clawhub/sharozdawa | ✅ HTML 页面组装与 Schema.org 注入（Product + FAQPage） |
| 7 | **seo-geo-qa** | clawhub/justinbao19 | ✅ 多维度内容质检（数据准确性、栏目完整度、关键词、Schema、Alt、销售力） |

---

## 🔒 锁定状态

所有技能已安装并配置完成，版本锁定。
**今后不再更换技能或调整配置**，确保每次生成的页面在结构和风格上完全统一。

---

## 🏭 流水线流程图

```
接收飞书文档
    ↓
[Step 1] 深度解析与链接学习
    └─→ markdown-new-crawl + feishu-fetch-doc
    └─→ 提取结构化数据 + 递归抓取所有链接内容
    ↓
[Step 2] 数据补充与网络搜索
    └─→ deep-search + miaoda-web-search
    └─→ 英文检索专业用法、行业案例
    ↓
[Step 3] 英文内容创作（GEO 优化）
    └─→ seo-geo-playbook
    └─→ 固定7栏目 + FAQ + 图片Alt描述
    ↓
[Step 4] 图片生成
    └─→ huoshan-ai-generator (SeaDream 5.0 Lite)
    └─→ 3-5张：棚拍特写 + 场景渲染图
    ↓
[Step 5] 样式模板应用
    └─→ html-analysis
    └─→ 学习并应用固定DOM结构、配色、字体
    ↓
[Step 6] 页面组装
    └─→ 内置HTML组装
    └─→ section包裹 + 响应式 + CTA按钮
    ↓
[Step 7] 结构化数据注入
    └─→ schema-gen
    └─→ JSON-LD: Product + FAQPage Schema
    ↓
[Step 8] 自检并询问补充 ⚠️ 暂停点
    └─→ seo-geo-qa (6项质检，1-10分)
    └─→ 展示初稿 + 等待用户补充输入
    ↓
[Step 9] 最终优化与交付
    └─→ 根据补充信息精准修改
    └─→ 再次质检 ≥9分 → 输出最终HTML
```

---

## ✅ 配置校验清单

| 校验项 | 状态 |
|--------|------|
| 技能安装完整（7个核心技能） | ✅ 完成 |
| 技能版本锁定 | ✅ 完成 |
| IDENTITY 品牌配置（Plastuf） | ✅ 完成 |
| SOUL 内在性格固化 | ✅ 完成 |
| 9步工作流固化 | ✅ 完成 |
| 所有输出使用英文 | ✅ 强制启用 |
| Plastuf 品牌名拼写校验 | ✅ 零容忍 |
| 技术参数不编造规则 | ✅ 严格执行 |
| 栏目顺序固定 | ✅ 不可调换 |
| Step 8 暂停等待机制 | ✅ 启用 |

---

## 🚀 就绪状态

✅ **配置完成，可随时接收飞书文档**

使用方式：
1. 用户发送一个产品的飞书 Markdown 文档
2. 详情页助手自动执行 Step 1-7
3. 生成初稿并询问用户是否需要补充
4. 用户回复补充或确认
5. 输出最终版 HTML

---

*本配置一次性完成，今后不再变动。*
*详情页助手已就绪，可随时接收飞书文档。*
