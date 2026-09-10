# Day_3 · CSS 选择器与颜色字体

> 预计耗时：20~30 分钟
> HTML 是骨架，CSS 是衣服。今天学会用**选择器**找到元素，再设置颜色和字体。

## 今日知识点

- CSS 三种写法：内联 `style="..."`、内部 `<style>`、外部 `<link>`（推荐外部）
- 选择器：标签选择器 `h1`、类选择器 `.类名`、id 选择器 `#id`
- 常用属性：`color` 文字颜色、`font-size` 字号、`background-color` 背景色、`text-align` 对齐

## 先学（教程）

- 菜鸟教程 CSS（看"CSS 语法"和"CSS 选择器"）：https://www.runoob.com/css/css-tutorial.html
- MDN·CSS 基础：https://developer.mozilla.org/zh-CN/docs/Learn/Getting_started_with_the_web/CSS_basics
- B站视频（黑马程序员，看讲"CSS 语法、标签/类/id 选择器、颜色字体"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

新建 `style.css` 和 `styled.html`，用**外部样式表**给 Day_1 的自我介绍页面加样式：

1. `<head>` 里用 `<link rel="stylesheet" href="style.css">` 引入
2. 标签选择器：给 `body` 设背景色、`h1` 设文字颜色
3. 类选择器：定义 `.highlight` 背景高亮，给某段文字加上
4. id 选择器：定义 `#title`，给标题设更大字号、居中

## 完成标准

- [ ] 外部样式表生效（改 style.css 页面就变）
- [ ] 标签/类/id 三种选择器都用到了
- [ ] 能说出 `.类名` 和 `#id` 的区别

**提交方式**：把 `styled.html` 和 `style.css` 代码贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!-- styled.html -->
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>关于我</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <h1 id="title">我叫张三</h1>
    <p class="highlight">我是web部的新成员。</p>
    <p>这是加过样式的页面。</p>
  </body>
</html>
```

```css
/* style.css */
body {
  background-color: #f0f0f0;
}

h1 {
  color: #2c7be5;
}

#title {
  font-size: 40px;
  text-align: center;
}

.highlight {
  background-color: yellow;
}
```
