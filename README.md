# academic-page

Peiyang Ni 的学术主页，基于 Jekyll（AcademicPages / Minimal Mistakes）。同一份内容发布在两个地址：

- 主地址：`https://bonjour-npy.github.io/`
- 兼容旧地址：`https://bonjour-npy.github.io/academic-page/`
- 博客：`https://bonjour-npy.github.io/blog/`

## 常用内容位置

- 主页正文与论文卡片：`_pages/about.md`
- 独立 Publications 页面：`_pages/publications.html`
- CV 页面：`_pages/cv.md`
- Publications 条目：`_publications/*.md`
- 主页样式：`_sass/layout/_homepage.scss`
- 顶部导航：`_data/navigation.yml`

## 本地预览主页

首次使用先安装依赖：

```bash
bundle install
```

以后直接启动：

```bash
bundle exec jekyll serve
```

浏览器打开 `http://localhost:4000/academic-page/`。修改 `_config.yml` 后需要重启服务。

## 更新并发布主页

先提交并推送本仓库，更新兼容旧地址：

```bash
git status
git add .
git commit -m "Update homepage"
git push origin master
```

然后进入相邻的根站仓库，把最新主页同步到根地址，同时重新发布 `/blog/`：

```bash
cd ../bonjour-npy.github.io
npm run deploy
```

`npm run deploy` 会读取相邻的 `../academic-page`，组合构建主页和博客，并把生成文件推送到根站仓库的 `gh-pages` 分支。它不会修改两个仓库的 `master` 源码。

## 预览完整根站

```bash
cd ../bonjour-npy.github.io
npm run build:combined
npm run serve:combined
```

浏览器打开 `http://localhost:4000/`，并检查 `/blog/`。停止预览按 `Ctrl-C`。

## 维护规则

- 只修改两个真实目录：`~/Codes/academic-page` 和 `~/Codes/bonjour-npy.github.io`。
- `academic-page/master` 是主页源码；推送后 GitHub Pages 自动更新 `/academic-page/`。
- `bonjour-npy.github.io/master` 是博客和部署脚本源码；`gh-pages` 只保存组合后的静态网站，不要手动编辑。
- 修改博客后，先提交并推送根站的 `master`，再执行 `npm run deploy`。
- 部署前两个仓库都必须没有未提交改动；脚本发现脏工作区会停止，避免发布不可复现的内容。
- 如果依赖缺失：本仓库运行 `bundle install`，根站仓库运行 `npm ci`。
