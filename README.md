# 高级 WebRTC 架构：从原理到实践

中文 WebRTC 架构学习电子书，共 **11 个部分、76 章**，涵盖 WebRTC 基础、网络与信令、编解码器、媒体服务器、设计模式、标准化、部署、测试与监控等主题。

正文使用 Markdown 编写，通过 MkDocs Material 提供分组目录、站内搜索和代码高亮。书中包含精选课程幻灯片及中文 SVG 示意图。

## 本地预览

### Windows（PowerShell）

```powershell
py -m venv .venv
.venv\Scripts\python -m pip install -r requirements.txt
.venv\Scripts\python -m mkdocs serve -a 127.0.0.1:8000
```

### Linux / macOS

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
.venv/bin/python -m mkdocs serve -a 127.0.0.1:8000
```

打开 <http://127.0.0.1:8000/>。

## 构建

```bash
python -m mkdocs build --strict
```

生成的网站位于 `site/`。若未激活虚拟环境，请将 `python` 替换为 `.venv\Scripts\python`（Windows）或 `.venv/bin/python`（Linux/macOS）。

## 发布到 GitHub Pages

仓库已提供 `.github/workflows/deploy.yml`。发布前请按实际地址在 `mkdocs.yml` 中设置：

```yaml
site_url: https://<你的用户名>.github.io/webrtc-architecture-ebook/
repo_url: https://github.com/<你的用户名>/webrtc-architecture-ebook
```

推送到 `main` 分支后，GitHub Actions 会构建并发布网站。仓库的 **Settings → Pages → Build and deployment → Source** 应选择 **GitHub Actions**。

## 内容说明

本书是 Advanced WebRTC Architecture 课程的结构化学习笔记，不替代原课程。原课程视频及幻灯片的权利归相应权利人所有，本书仅作为学习整理材料。涉及浏览器支持、产品能力和标准状态的内容具有时效性，请查阅最新官方资料。
