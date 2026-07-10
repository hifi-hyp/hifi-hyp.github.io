# 个人网站 (Personal Website)

一个简约、无需构建工具的学术风格个人主页，托管在 GitHub Pages。

## 文件结构

```
.
├── index.html        # 主页面 —— 你主要编辑这个文件（内容都在里面，带 EDIT 注释）
├── styles.css        # 样式（颜色、字体、间距都在最上面的变量里）
├── favicon.svg       # 浏览器标签页的小图标
├── assets/
│   ├── profile.svg   # 头像占位图 —— 换成你自己的照片
│   └── cv.pdf        # （放入你的 CV，index.html 里 CV 链接指向这里）
└── README.md
```

## 如何修改内容

打开 `index.html`，搜索 `EDIT` 注释，按提示替换：
- **姓名 / 头衔 / 单位**：`HERO` 区域
- **链接**：邮箱、Google Scholar、GitHub、LinkedIn、CV —— 把 `YOUR-USERNAME` 和 `you@example.com` 换成你的
- **About / News / Publications / Experience / Education**：各 `section`
- 用不到的链接或板块，直接删掉对应的整段即可

**换头像**：把你的照片命名为 `profile.jpg` 放进 `assets/`，然后把 `index.html` 里的
`assets/profile.svg` 改成 `assets/profile.jpg`。

**改配色/字体**：编辑 `styles.css` 顶部 `:root` 里的变量（比如把 `--accent` 换成别的颜色）。

## 本地预览

直接双击 `index.html` 用浏览器打开即可。

## 部署到 GitHub Pages

网站仓库命名为 `<你的用户名>.github.io`，推送到 GitHub 后会自动发布在
`https://<你的用户名>.github.io`。详细步骤见对话记录。

修改后重新发布：
```bash
git add -A
git commit -m "Update site"
git push
```
推送后等待约 1 分钟即可生效。
