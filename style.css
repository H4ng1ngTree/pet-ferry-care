# 毛孩子的“摆渡人”

这是一个可直接部署到 GitHub Pages 的静态数据新闻页面模板。

## 文件结构

```text
pet-ferry-github-page/
├── index.html          # 页面正文
├── style.css           # 页面样式
├── assets/             # 图片、图表、封面图目录
├── data/               # CSV/XLSX/Markdown 数据与资料文件
└── README.md           # 部署说明
```

## 本地预览

最简单的方法：双击 `index.html`。

如果想用本地服务器预览，在该目录下运行：

```bash
python -m http.server 8000
```

然后打开：

```text
http://localhost:8000
```

## 更新图片和图表

页面已经放入了根据现有数据生成的 SVG 图表，以及你提供的 JPG 图表。后续如果拿到更正式的制图版本，可以直接替换 `assets/` 中的同名文件。

如果要新增图片，可以使用这种写法。

```html
<figure class="figure">
  <img src="./assets/你的图表文件名.png" alt="图表说明">
  <figcaption>数据来源：写清楚来源和统计口径。</figcaption>
</figure>
```

当前主要图片命名：

```text
assets/
├── chart-01-demand-gap.svg
├── chart-02-survey-findings.svg
├── chart-03-motivation-wordcloud.svg
├── company-region-map.jpg
├── company-region-share.jpg
├── chart-05-industry-problems.svg
├── cremation-rate-trend.jpg
├── service-choice-items.jpg
├── chart-08-policy-timeline.svg
├── chart-09-country-comparison.svg
└── chart-10-governance-path.svg
```

可继续补充的图片命名：

```text
assets/
├── hero-cover.jpg
├── chart-01-demand-gap.png
├── chart-02-survey-findings.png
├── chart-03-worker-profile.png
├── chart-04-company-growth.png
├── chart-05-industry-problems.png
├── chart-06-public-service.png
├── chart-07-policy-timeline.png
├── chart-08-country-comparison.png
└── chart-11-interview-photo.png
```

## 部署到 GitHub Pages

1. 新建一个 GitHub 仓库，比如 `pet-ferry-news`。
2. 把本文件夹里的 `index.html`、`style.css`、`assets/`、`data/`、`README.md` 上传到仓库根目录。
3. 进入仓库页面，点击 `Settings`。
4. 左侧找到 `Pages`。
5. 在 `Build and deployment` 里：
   - `Source` 选择 `Deploy from a branch`
   - `Branch` 选择 `main`
   - 文件夹选择 `/root`
6. 保存后等待 1-3 分钟。
7. GitHub 会生成访问链接，一般格式是：

```text
https://你的用户名.github.io/pet-ferry-news/
```

## 用 Git 命令上传

如果你本地已经安装 Git，可以这样操作：

```bash
git init
git add .
git commit -m "add pet ferry data news page"
git branch -M main
git remote add origin https://github.com/你的用户名/pet-ferry-news.git
git push -u origin main
```

推送完成后，按上面的 GitHub Pages 步骤开启页面即可。

## 参赛前检查清单

- 所有图表都写明数据来源和口径。
- 问卷样本量、样本结构、局限性写清楚。
- 已嵌入页面的数据表对应源文件位于 `data/`。
- 图片文件名不要用空格，尽量使用英文或拼音。
- 浏览器打开页面，检查手机端和电脑端都不溢出。
- GitHub Pages 链接能正常访问。
