# Portfolio Audit Report

生成时间：2026-08-15

## 已完成

- 已将 `E:\桌面\havoury` 隔离为独立 Git 仓库。
- 已推送 GitHub Profile 仓库 `havoury/havoury`。
- 已验证远程 `README.md` 存在于 `main` 分支。
- 已建立本地 Academic Portfolio 仓库 `E:\桌面\havoury.github.io`。
- 已完成静态个人主页第一版，包含 Home、About、Research Interests、Publication、Selected Projects、Experience、Contact。
- 已推送 GitHub Pages 仓库 `havoury/havoury.github.io`。
- 已验证 `https://havoury.github.io` 返回 HTTP 200。
- 已审计原始 ECAYOLOv8n-LC 本地工作目录，发现不能直接公开的敏感和大体积内容。
- 已建立清理后的本地公开候选仓库 `E:\桌面\ecayolov8n-lc`，并完成初始提交。
- 已建立可维护数据结构：
  - `data/publications.json`
  - `data/projects.json`
- 已检查 `data/*.json` 可解析。
- 已将 `havoury/` 和 `havoury.github.io/` 从上级桌面 Git 仓库忽略，避免仓库边界污染。

## 当前 GitHub 状态

### `havoury/havoury`

- 状态：已创建并已推送。
- 默认分支：`main`
- 当前用途：GitHub Profile README。
- 远程验证：`README.md` 和 `PORTFOLIO_TODO.md` 均可通过 GitHub 集成读取。

### `havoury/havoury.github.io`

- 状态：已创建并已推送。
- 本地状态：已完成第一版静态站点并提交。
- 本地 commit：`822b426 Initialize academic portfolio site`
- 部署地址：`https://havoury.github.io`

## 内容策略检查

- Profile README 使用英文主体，适合 GitHub 对外展示。
- 中文内容仅用于本地维护文档和审计记录。
- 已避免 GitHub Stats、Visitor Counter、大量 Badge、Typing Animation 等低价值装饰。
- 已突出主线：Computer Vision / Efficient AI / Intelligent Systems。
- 已优先展示经过用户确认的论文、项目身份、指标和奖项信息。

## 真实性约束检查

- 未新增未经确认的论文、奖项、项目时间、实验指标或作者身份。
- 团队/项目身份按已确认信息标注：
  - ECAYOLOv8n-LC：Sole Author
  - OpenHarmony + RK3566：Project Lead
  - Smart Community Microservices：Project Lead
  - NTU AI Project：访学项目经历，未夸大为独立科研成果

## ECAYOLOv8n-LC 审计结论

- 原目录具有高 Portfolio 价值，但不能直接公开。
- 已发现并排除：本地访问凭据、虚拟环境、数据集、cache、checkpoints、训练生成物、绝对路径数据清单。
- 已抽取并参数化：数据划分脚本、YOLOv8-seg 数据转换脚本、U-Net baseline 脚本。
- 当前公开候选仓库仍是 scaffold，需要继续补齐 ECAYOLOv8n-LC 方法实现和可公开实验材料。

## 技术检查

- Profile 仓库为普通 Markdown，无构建步骤。
- Pages 仓库为静态 HTML/CSS/JSON，无构建步骤。
- `index.html` 已包含 viewport、description、语义化 section、导航 aria-label。
- 当前外部链接仅包含 `https://github.com/havoury`，风险低。
- GitHub Pages 兼容性：静态根目录 `index.html` 可直接部署。

## 待处理

- 创建远程仓库 `havoury.github.io`。
- 检查 `https://havoury.github.io` 的桌面端和移动端视觉效果。
- 将 Profile README 中的 Academic portfolio 链接改为 `https://havoury.github.io`。
- 创建并推送远程仓库 `havoury/ecayolov8n-lc`。
- 后续审计 OpenHarmony + RK3566、NTU AI Project、Smart Community Microservices 等项目仓库。
