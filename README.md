# 毛孩子的“摆渡人”

这是一个可直接部署到 GitHub Pages 的静态数据新闻页面模板。

## 文件结构

```text
pet-ferry-github-page/
├── index.html          # 页面正文
├── style.css           # 页面样式
├── assets/             # 图片、图表、封面图占位目录
├── data/               # CSV/Excel/JSON 等数据文件占位目录
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

## 替换图片和图表

页面现在使用的是“占位卡”。后续拿到正式图片或图表后，有两种替换方式。

方式一：继续用占位卡，只改文字。

```html
<div class="visual-slot">
  <div>
    <b>图表占位 01</b>
    <span>核心矛盾：宠物规模、离世规模与殡葬渗透率</span>
  </div>
</div>
```

方式二：替换成真实图片。

```html
<figure class="figure">
  <img src="./assets/你的图表文件名.png" alt="图表说明">
  <figcaption>数据来源：写清楚来源和统计口径。</figcaption>
</figure>
```

建议图片命名：

```text
assets/
├── hero-placeholder.jpg
├── chart-01-demand-gap.png
├── chart-02-survey-findings.png
├── chart-03-worker-profile.png
├── chart-04-company-growth.png
├── chart-05-industry-problems.png
├── chart-06-public-service.png
├── chart-07-policy-timeline.png
├── chart-08-country-comparison.png
└── chart-09-governance-path.png
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
- 图片文件名不要用空格，尽量使用英文或拼音。
- 浏览器打开页面，检查手机端和电脑端都不溢出。
- GitHub Pages 链接能正常访问。
