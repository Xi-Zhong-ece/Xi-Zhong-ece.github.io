# Xi Zhong — Academic Homepage

Source for **https://xi-zhong-ece.github.io**

纯静态站点：没有 Jekyll、没有构建流程、没有 GitHub Actions。
push 到 `main` 之后 GitHub Pages 直接发布，几十秒生效。

## 文件

| 文件 | 作用 |
| --- | --- |
| `index.html` | 整个网站的内容（所有章节都在这一个文件里） |
| `style.css` | 所有样式；颜色和字号集中在文件顶部的 `:root` 变量里 |
| `assets/img/prof_pic.jpg` | 头像（换照片保持同名即可） |
| `assets/pdf/Xi_Zhong_CV.pdf` | CV（换 PDF 保持同名即可） |
| `.nojekyll` | 告诉 GitHub Pages 不要用 Jekyll 处理，原样发布 |

## 怎么改

**加一条 news** — 在 `index.html` 里找到 `<table class="news">`，照着现有的复制一行：

```html
<tr>
  <td class="date">Oct. 2026</td>
  <td>这里写内容，链接用 <a href="网址">文字</a>。</td>
</tr>
```

**加一篇论文** — 找到对应的 `<table class="pubs">`（Conference / Journal / Manuscripts），复制一行改内容。
自己的名字用 `<u>X. Zhong</u>` 包起来会显示下划线，期刊/会议名用 `<i>...</i>` 显示斜体。

**改配色 / 字号** — 打开 `style.css`，最上面的 `:root` 里：

- `--heading-name` 顶部姓名的蓝色
- `--heading-section` 小节标题的深红色
- `--link` 链接蓝色
- `--size-body` 正文字号
- `--font-body` 字体

**加中文名** — `index.html` 里 `<h1 id="home">` 上方有注释说明。

**加一个新章节** — 复制一段 `<h3 id="xxx">标题</h3>`，再去左侧 `<nav class="sidebar">` 里加一条
`<li><a href="#xxx">标题</a></li>`。

## 发布

在 GitHub Desktop 里 Commit → Push origin，等几十秒刷新网页即可。
如果没变化，按 `Command + Shift + R` 强制刷新绕过浏览器缓存。
