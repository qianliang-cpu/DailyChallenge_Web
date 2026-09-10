# Day_4 · CSS 盒模型：每个元素都是一个"盒子"

> 预计耗时：20~30 分钟
> 布局最核心的概念：每个元素都是个盒子，由内容、内边距、边框、外边距四层组成。

## 今日知识点

- 四层（由内到外）：`content`（内容）→ `padding`（内边距）→ `border`（边框）→ `margin`（外边距）
- 常用：`margin`、`padding`、`border: 1px solid 颜色`、`border-radius`（圆角）

## 先学（教程）

- 菜鸟教程 CSS（看"CSS 盒子模型"）：https://www.runoob.com/css/css-boxmodel.html
- MDN·盒模型：https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Building_blocks/The_box_model
- B站视频（黑马程序员，看讲"盒子模型、padding/border/margin"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

新建 `box.html`：

1. 写两个 `div`（class 为 `box1`、`box2`），各放一句话
2. 给 `.box1` 设 `width: 200px`、`padding: 20px`、`border: 5px solid black`、`margin: 30px`
3. 用 F12 看看它的**总宽度**是多少（200 + 20×2 + 5×2 = 250）
4. 给 `.box2` 加 `border-radius: 10px` 圆角和背景色

## 完成标准

- [ ] 能说清楚 padding / border / margin 各自作用
- [ ] 能算出盒子总宽度 250
- [ ] 圆角效果正常

**提交方式**：把 `box.html` 代码 + 你算出的总宽度，贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>盒模型</title>
    <style>
      .box1 {
        width: 200px;
        padding: 20px;
        border: 5px solid black;
        margin: 30px;
        background-color: lightblue;
      }
      .box2 {
        width: 200px;
        padding: 20px;
        border: 5px solid black;
        margin: 30px;
        background-color: lightcoral;
        border-radius: 10px;
      }
    </style>
  </head>
  <body>
    <div class="box1">盒子 1</div>
    <div class="box2">盒子 2（圆角）</div>
  </body>
</html>
```
