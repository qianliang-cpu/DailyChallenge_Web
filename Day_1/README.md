# Day_1 · HTML 文档结构与常用标签

> 预计耗时：20~30 分钟
> HTML 是网页的"骨架"。今天认识一个页面的基本结构，和几个最常用的标签。

## 今日知识点

- HTML 文档结构：`<!DOCTYPE html>`、`<html>`、`<head>`、`<body>`
- 常用标签：标题 `<h1>`~`<h6>`、段落 `<p>`、链接 `<a>`、图片 `<img>`
- 盒子标签：`<div>`（块级容器）、`<span>`（行内容器）

## 先学（教程）

- 菜鸟教程 HTML（看"HTML 简介"和"HTML 元素"）：https://www.runoob.com/html/html-tutorial.html
- MDN·HTML 基础：https://developer.mozilla.org/zh-CN/docs/Learn/Getting_started_with_the_web/HTML_basics
- B站视频（黑马程序员，看讲"HTML 结构、标题/段落/div/span/图像/链接标签"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

新建 `about.html`，写一个自我介绍页面：

1. 完整文档结构（`<!DOCTYPE html>`、`<html>`、`<head>`、`<body>` 一个不少）[注:打一个!再按tab键可以直接补齐html骨架]
2. 一个 `<h1>` 主标题、两个 `<p>` 段落介绍自己
3. 一个 `<a>` 链接（用 `target="_blank"`）、一张 `<img>` 图片
4. 用 `<div>` 包住一段内容、用 `<span>` 给一句话占位（今天先不写样式）

示例骨架：
```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>关于我</title>
  </head>
  <body>
    <h1>我叫张三</h1>
    <div>
      <p>我是web部的新成员。</p>
      <span>这句话稍后要变色。</span>
    </div>
  </body>
</html>
```

> `lang="zh"` 表示中文，`<meta charset="UTF-8">` 防止中文乱码。

## 完成标准

- [ ] 页面能正常打开，中文不乱码
- [ ] h1/p/a/img/div/span 都用到了
- [ ] 能说出 `<head>` 和 `<body>` 分别放什么

**提交方式**：把 `about.html` 代码贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>关于我</title>
  </head>
  <body>
    <h1>我叫张三</h1>
    <div>
      <p>我是web部的新成员，来自青岛，喜欢写代码。</p>
      <p>这是我做的第一个网页。</p>
    </div>
    <a href="https://www.runoob.com" target="_blank">我的学习资料</a>
    <img src="https://www.runoob.com/wp-content/uploads/2013/12/react.png" alt="图片" width="200">
  </body>
</html>
```
