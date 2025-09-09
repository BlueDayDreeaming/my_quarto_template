# 我的 Quarto 书籍模板

这是一个基于 Quarto 的书籍模板，可以用来快速创建自己的在线电子书。

## 快速开始

1. **安装 Quarto**：从 [Quarto 官网](https://quarto.org/docs/get-started/) 下载并安装

2. **克隆或下载模板**：
   ```bash
   git clone your-repo-url
   cd your-book-name
   ```

3. **自定义配置**：
   - 编辑 `_quarto.yml` 文件，修改书名、作者、网址等信息
   - 替换 `images/` 目录中的 logo 和封面图片
   - 修改 `index.qmd` 首页内容

4. **编写内容**：
   - 在 `body/` 目录下编写你的章节内容
   - 支持 Markdown (`.md`) 和 Jupyter Notebook (`.ipynb`) 格式
   - 在 `_quarto.yml` 中更新章节列表

5. **预览和发布**：
   ```bash
   quarto render        # 生成 HTML 文件
   quarto preview      # 本地预览
   ```

## 文件结构

```
my_quarto_template/
├── _quarto.yml          # 配置文件
├── index.qmd           # 首页
├── styles.css          # 自定义样式
├── body/               # 章节内容
│   ├── chapter1.md
│   ├── chapter2.md
│   ├── chapter3.md
│   ├── chapter4.ipynb
│   └── appendix.md
└── images/             # 图片资源
    ├── book-logo.png
    └── book-front.png
```

## 自定义指南

### 1. 修改书籍信息
在 `_quarto.yml` 中修改：
- `title`: 书名
- `author`: 作者
- `site-url`: 网站地址
- `tools.href`: GitHub 仓库地址

### 2. 组织章节
在 `_quarto.yml` 的 `chapters` 部分组织你的内容：
- 使用 `part` 创建部分
- 列出章节文件路径
- 支持 `.md` 和 `.ipynb` 文件

### 3. 自定义样式
- 编辑 `styles.css` 自定义外观
- 在 `_quarto.yml` 中选择主题：`cosmo`, `flatly`, `litera` 等

## 发布到 GitHub Pages

1. 将代码推送到 GitHub 仓库
2. 在仓库设置中启用 GitHub Pages
3. 选择 `docs` 文件夹作为源
4. 访问 `https://your-username.github.io/your-repo-name/`

## 需要修改的地方

使用此模板时，请修改以下内容：
- [ ] `_quarto.yml` 中的所有个人信息
- [ ] `index.qmd` 中的首页内容
- [ ] `images/` 目录中的图片文件
- [ ] 各章节的实际内容
- [ ] GitHub 仓库相关的链接
