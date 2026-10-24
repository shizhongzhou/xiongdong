# 一头熊的熊洞 · 摄影作品集

个人摄影作品集网站，纯静态页面，无需构建，直接打开 `index.html` 即可浏览。

## 目录结构

```
index.html          网站首页（可直接部署）
images/             照片素材
  hero.jpg          首页封面大图
design/             Claude 设计画布的源文件（用于存档和继续编辑）
  Main.dc.html
  canvas.json
```

## 用 GitHub Pages 免费上线

1. 打开本仓库的 **Settings → Pages**
2. Source 选择 **Deploy from a branch**，分支选 `main`，目录选 `/ (root)`，保存
3. 一两分钟后，网站会出现在 `https://<你的用户名>.github.io/<仓库名>/`

## 添加照片

1. 把照片放进 `images/` 文件夹
2. 在 `index.html` 里找到对应的占位框（例如「照片 01 · 竖幅 4:5」），把那个 `<div>` 换成：

```html
<img src="images/你的照片.jpg" alt="照片描述" style="width: 100%; aspect-ratio: 4 / 5; object-fit: cover; display: block">
```

## 当前设置

- 标题字体：思源宋体（Noto Serif SC）
- 正文字体：思源黑体 Light（Noto Sans SC）
- 点缀色：`#C9A46A`
- 封面高度：860px
