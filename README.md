# TL.github.io

个人简历静态网站。

## 修改简历内容

日常更新只需要编辑 [`resume-data.js`](resume-data.js)：

- `profile`：姓名、个人简介、照片和联系方式。
- `sections.overview`：研究概述。
- `sections.education.items`：教育经历。
- `sections.papers.items`：学术论文。
- `sections.projects.items`：科研项目。
- `sections.skills.items`：专业技能。
- `sections.honors.categories`：获奖情况。
- `sections.service.items`：学术兼职。
- `footer`：页脚信息。

每个模块都有 `enabled` 开关。设为 `false` 后，该模块及其导航入口都会隐藏。

论文条目的核对来源保存在 `sections.papers.sourceUrl`。修改作者、标题、期刊或年份时，应以 Google Scholar、出版社或 DOI 页面为准，不要根据标题猜测缺失信息。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| `resume-data.js` | 所有可编辑的简历数据 |
| `index.html` | 页面入口，通常不需要修改 |
| `script.js` | 将简历数据生成到页面中 |
| `style.css` | 页面样式和移动端布局 |
| `photo.jpg` | 个人照片，替换时请保持文件名不变 |
| `assets/projects/` | 科研项目展示图片 |

## 本地预览与发布

直接打开 `index.html` 即可预览。确认无误后提交到 `main` 分支，GitHub Pages 会自动更新：

```powershell
git add index.html resume-data.js script.js style.css README.md
git commit -m "Update resume content"
git push origin main
```
