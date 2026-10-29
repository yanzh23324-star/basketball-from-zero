# 第一球 · 从零开始打篮球

[打开网站](https://yanzh23324-star.github.io/basketball-from-zero/)

参考「第一脚」足球入门站的多页面学习结构，制作的中文篮球入门网站。5 个板块、18 节独立短课、29 个页面，包含课程搜索、收藏、已读进度、规则自测、三步接应图解和可导出的本地练习笔记。

## 本地构建

```sh
python3 scripts/build.py
python3 -m http.server 8000 --directory site
```

内容在 `content/lessons.json`，页面由 `scripts/build.py` 生成。修改后重新构建，将 `site/` 内全部内容复制到仓库根目录再提交。GitHub Pages 从 main 根目录发布。

- `assets/`：样式与浏览器交互源码。
- `scripts/content.py`：首版内容生成底稿；日常修改直接编辑 JSON，无需运行此脚本。
- 所有学习数据仅存于当前浏览器 localStorage，不上传、不同步，笔记支持 JSON 导出。
- 无账号、无后端、无付费 API。

规则按 FIBA 体系整理；正式三人篮球与普通半场野球分别说明。资料链接和适用范围见网站来源页。练习为本站编排，可按状态降低难度。
