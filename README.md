# Dotty Tutor — 静态网页 Demo

基于 PRD 生成的产品演示网页，纯前端（HTML + TailwindCSS CDN + 原生 JS），所有数据均为 mock，不接入真实 MinerU / 大模型接口。

## 页面说明
- `login.html` / `index.html` — 登录页（可切换"教研管理员 / 学生"身份）
- `teacher-dashboard.html` — 教研工作台首页
- `upload.html` — 教材上传 + MinerU OCR 处理进度模拟
- `review.html` — AI 出题 & 双模型审校 + 质量门禁结果 + 人工编辑
- `bank.html` — 题库管理（筛选/检索）
- `student-home.html` — 学生首页
- `practice.html` — 答题练习（7 种题型：单选/多选/判断/填空/简答/匹配/拖拽排序，分层提示）
- `mistakes.html` — 错题复盘 + 多轮陪练入口

## 本地预览
直接双击 `login.html` 或 `index.html` 在浏览器中打开即可，无需安装依赖或启动服务。

## 部署到 GitHub Pages
1. 新建一个 GitHub 仓库，把本文件夹内所有文件（含 `assets/`）推送到仓库根目录（或 `docs/` 目录）。
2. 仓库 Settings → Pages → Source 选择对应分支 / 目录 → Save。
3. 稍等片刻后，GitHub 会给出访问链接，默认入口页是 `index.html`（即登录页）。

## 技术说明
- 样式：TailwindCSS（CDN 版）+ `assets/style.css` 中的设计变量（颜色、圆角、卡片、按钮等）
- 数据：`assets/data.js` 中的 `DOTTY_DATA`，修改这里的对象即可替换演示内容
- 无构建步骤、无后端依赖，纯静态文件，可直接托管在任意静态网站服务上
