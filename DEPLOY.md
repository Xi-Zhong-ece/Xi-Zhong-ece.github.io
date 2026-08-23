# 部署说明（首次）

目标仓库：`Xi-Zhong-ece/Xi-Zhong-ece.github.io`
目标网址：https://xi-zhong-ece.github.io

## 1. 用本包内容替换仓库内容

1. 把本压缩包解压，得到的所有文件和文件夹（**包括隐藏的 `.github` 文件夹**）放到仓库根目录，替换原有内容。
   - macOS Finder 中按 `Command + Shift + .` 可显示隐藏文件；或者直接用 GitHub Desktop / 命令行，隐藏文件会自动包含。
   - 建议先删除仓库里旧的文件（`DEPLOYMENT_INSTRUCTIONS.md`、`DEPLOY_WORKFLOW_COPY.yml`、`_pages/research.md`、`assets/profile.jpg` 等），避免残留。
2. 命令行方式（推荐）：

   ```bash
   git clone https://github.com/Xi-Zhong-ece/Xi-Zhong-ece.github.io.git
   cd Xi-Zhong-ece.github.io
   git rm -rq . && rm -rf ./* .github      # 清空旧内容（保留 .git）
   unzip -o ~/Downloads/Xi-Zhong-ece.github.io.zip -d .   # 解压本包到当前目录
   git add -A
   git commit -m "Rebuild site with al-folio and CV content"
   git push origin main
   ```

## 2. GitHub 设置（只需做一次）

1. 仓库 **Settings → Actions → General → Workflow permissions**：选 **Read and write permissions**，保存。
2. push 之后打开 **Actions** 标签页，等待 **Deploy site** 工作流跑完（首次约 3–5 分钟）。成功后会自动生成 `gh-pages` 分支。
3. 仓库 **Settings → Pages**：**Build and deployment → Source** 选 **Deploy from a branch**，分支选 **gh-pages**，目录 **/(root)**，保存。
4. 等一两分钟后访问 https://xi-zhong-ece.github.io 。

如果 Actions 失败，点进失败的运行查看日志；最常见原因是第 1 步的 Workflow permissions 没有打开。

## 3. 日常更新

- 改简介：`_pages/about.md`
- 加论文：在 `_bibliography/papers.bib` 增加 BibTeX 条目（`abbr` 用于左侧彩色徽章，`selected = {true}` 会显示在首页）
- 改 CV 页面：`_data/cv.yml`；替换 PDF：`assets/pdf/Xi_Zhong_CV.pdf`
- 加新闻：在 `_news/` 里新建 `YYYY-MM-DD-xxx.md`（格式参考现有文件）
- 换照片：替换 `assets/img/prof_pic.jpg`

每次 push 到 `main` 都会自动重新构建并发布。
