---
# 搜索页 Front Matter
# 该页面使用主题提供的 search 布局渲染站内搜索框
title: "搜索"
layout: "search"            # 指定使用 layouts/search.html 模板
description: "搜索本站文章"
# placeholder：搜索框占位提示文字
placeholder: "输入关键词后回车..."
# weight：在菜单/列表中的权重（数字越小越靠前）
weight: 30
# 这个页面不需要显示在归档列表里
draft: false
---

<!-- 
  注意：此页面正文留空即可。
  实际的搜索 UI、搜索框、结果容器都由主题的 layouts/search.html 模板渲染。
  这里 front matter 的 layout: "search" 是关键，
  Hugo 会跳过默认 single.html，改用 search.html 渲染本页。

  搜索工作原理（前端无后端依赖）：
  1. Hugo 构建时根据 layouts/index.json 输出 index.json（依赖 hugo.toml 中 [outputs] home = [..., "JSON"]）
  2. 主题加载 assets/js/fuse.basic.min.js（Fuse.js 模糊搜索库）
  3. assets/js/fastsearch.js 监听搜索框输入，从 index.json 拉取数据后用 Fuse.js 检索
  4. 将匹配结果（标题、摘要、链接）渲染到结果容器
-->
