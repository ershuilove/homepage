# 个人学术主页 · GitHub 上传专用版

本版本专为 **GitHub 网页上传**制作：已移除超过 25MB 单文件上传限制的合集 PDF，
现在**所有文件均小于 5MB**，可以直接在浏览器里拖拽上传，不需要命令行。

```
李瀚源学术主页-GitHub版/
├── index.html   ← 主页（所有论文可点击）
├── papers/      ← 18 份论文 PDF（单篇 0.3~5MB）
└── 发布指南-GitHub版.md
```

> 如需保留「一键下载 256 页合集」按钮，请改用「李瀚源学术主页-发布版.zip」+
> 命令行 git 推送（git 单文件上限 100MB），或用 Netlify Drop 拖 zip 发布。

## 上传步骤（纯网页，约 3 分钟）

1. GitHub 登录 → 右上角 `+` → `New repository`
   - 仓库名：如 `homepage`
   - 选 **Public**（免费版 Pages 必须公开）
   - **不要勾选** Add a README / .gitignore / License（保持空仓库）
   - `Create repository`
2. 在仓库页面点 `Add file` → `Upload files`
3. 打开本文件夹，**全选里面的内容**（index.html + papers 文件夹 + 本文件）
   一起拖进上传框；确认文件列表里能看到 `papers/` 开头的路径
4. 点 `Commit changes`，等上传完成（18 份 PDF 共 33MB，约 1 分钟）

## 开启公开访问（GitHub Pages）

1. 仓库 `Settings` → 左侧 `Pages`
2. Branch 选 `main`，目录选 `/(root)` → `Save`
3. 约 1 分钟后，访问 `https://你的用户名.github.io/homepage/`

## 以后更新

网页方式：打开仓库里的 `papers` 文件夹 → `Add file` → `Upload files` →
拖入新 PDF（同名会自动替换）→ `Commit changes`。

命令行方式：在文件夹里执行

```bash
git add .
git commit -m "更新"
git push
```

## 已验证

- 18 个本地 PDF 链接全部有效（0 缺失）
- 最大单文件 5.0MB（遂宁 SSR 论文），全部低于 25MB 网页上传限制
- 主页其余功能（论文列表、DOI 外链、筛选按钮）与完整版完全一致
