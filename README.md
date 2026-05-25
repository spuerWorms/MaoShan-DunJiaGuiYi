# 遁甲归一 (Dunjia Guiyi) - 茅山奇门专业排盘与天文引擎

## 项目简介
“遁甲归一”是一个基于高精度天文历法（寿星天文）结合传统茅山奇门遁甲构建的专业级排盘与推演系统。项目通过严谨的物理场能量参数（经纬度、真太阳时、节气与七十二候），确立绝对精准的时空锚点，并内置自动化格局解析链路（COT）。

## 核心特性
* **高精度天文内核**：底层集成 `shouxing-engine.js` 与 `AstroKernel.js`，实现毫秒级的二十四节气交接与星历计算。
* **正统茅山奇门引擎**：`DunJiaKernel.js` 提供底层排盘逻辑，确保起局严谨。
* **时空动态校准**：通过 IP 自动定位（`dunjia_ipapi-full.html`），精准计算当地真太阳时，拒绝时间误差。
* **COT 深度解析链路**：内置 `qimen_interpreter.js`，并衍生出 `Glory-COT增强版` 与 `COT增强版` 等深度UI视图，实现自动化的奇门格局链路审计与智能解读。
* **移动端全面适配**：采用 Mobile-First 响应式设计策略，支持多断点布局（359px/360-479px/480-767px/768px+），触控交互优化（48dp 最小触控区域），确保在 iOS 和 Android 主流机型上提供一致体验。

## 目录与核心文件说明
项目分为 `/Docs` (文档)、`/Release` (发布版) 和 `/Source` (源码) 三个主要目录。

### 核心逻辑驱动 (JS)
* `shouxing-engine.js` / `AstroKernel.js`：底层天文物理量计算引擎。
* `DunJiaKernel.js` / `Formula.js`：遁甲核心算法与生克制化公式。
* `qimen_interpreter.js`：奇门格局智能解析器。
* `bundle.js`：打包后的全量核心依赖。

### 核心视图应用 (HTML)
* `qimen_calendar_modified_full - 内嵌数据版.html`：奇门万年历与排盘一体化稳定单文件。
* `Glory-COT增强版.html` / `COT增强版.html`：包含思维链（COT）与复杂解析逻辑的进阶排盘界面。
* `index.html`：项目标准主入口（配合弹窗与日历交互，已全面适配移动端）。

### 样式与工具
* `mobile-responsive.css`：移动端响应式样式文件（Mobile-First 策略，独立于原始样式）。
* `responsive-logger.js`：开发调试用断点监听与日志记录工具（生产环境已禁用）。

### 脚本与文档
* `optimize_qimen_interpreter.py`：解析器规则优化与生成脚本。
* `最新版更新说明操作步骤.txt` / `“遁甲归一”项目问题解决复盘.txt`：项目演进与维护日志。

## 部署与使用
本项目为纯前端架构设计（HTML/JS），无需配置复杂的后端环境。
1. 下载或克隆本仓库。
2. 推荐直接在浏览器中打开根目录的 `index.html` 或 `Glory-COT增强版-single.html` 进行本地使用。
3. **在线体验地址**：[https://weig19364.github.io/maoshanqimen/](https://weig19364.github.io/maoshanqimen/)

## 开发者
**卫光辉 (Glory Wei)** IT 系统架构师 / 专业数术研究者
