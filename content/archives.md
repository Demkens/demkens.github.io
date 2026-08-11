---
# 归档页 Front Matter
# 该页面使用主题提供的 archives 布局按时间线列出全部文章
title: "归档"
layout: "archives"          # 指定使用 layouts/archives.html 模板
description: "按时间线查看本站全部文章"
weight: 20
draft: false
---

<!-- 
  注意：此页面正文留空即可。
  实际归档列表由主题的 layouts/archives.html 模板渲染。

  归档页工作原理：
  1. 模板调用 Hugo 内置的 .Site.RegularPages 获取全部常规文章
  2. 按文章的 .Date 字段（发布日期）降序排列
  3. 按年份分组，输出形如 "2026 / 2025" 的分组标题
  4. 每组下列出该年所有文章的标题（可点击跳转）与发布日期

  影响 archives 页面内容的设置：
  - hugo.toml 中的 buildDrafts：true 时草稿也会出现在归档列表
  - 单篇文章 front matter 中的 date / publishDate 字段决定排序
  - 单篇文章 front matter 中的 archived: true 可将文章从归档中排除
-->
