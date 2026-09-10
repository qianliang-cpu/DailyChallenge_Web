# Day_5 · Flexbox：让元素乖乖排成一行

> 预计耗时：20~30 分钟
> 现在最常用的布局方式。今天学会用 flex 把几个元素排成一行、居中对齐。

## 今日知识点

- `display: flex` 开启弹性布局
- 主轴方向：`flex-direction: row`（横向，默认）/ `column`（纵向）
- 对齐：`justify-content`（center / space-between）、`align-items`（center）
- 间距：`gap`

## 先学（教程）

- 阮一峰·Flex 布局教程（图文并茂，重点看）：https://www.ruanyifeng.com/blog/2015/07/flex-grammar.html
- 菜鸟教程 CSS 弹性盒子：https://www.runoob.com/css/css3-flexbox.html
- B站视频（黑马程序员，看讲"flex 布局、justify-content/align-items"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

新建 `flex.html`：

1. 一个 `display: flex` 容器，里面放 3 个彩色方块
2. 用 `justify-content: space-between` 让它们两端对齐、均匀分布
3. 用 `gap: 20px` 拉开间距
4. 再做一个容器，用 `justify-content: center` + `align-items: center` 让一个方块**水平垂直居中**

## 完成标准

- [ ] 3 个方块能排成一行并均匀分布
- [ ] 能做出水平垂直居中
- [ ] 能说出 justify-content 和 align-items 分别管什么

**提交方式**：把 `flex.html` 代码 + 效果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>Flexbox</title>
    <style>
      .row {
        display: flex;
        justify-content: space-between;
        gap: 20px;
        background-color: #eee;
        padding: 10px;
      }
      .box {
        background-color: steelblue;
        color: white;
        padding: 20px;
      }
      .center {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 200px;
        background-color: #ddd;
        margin-top: 20px;
      }
    </style>
  </head>
  <body>
    <div class="row">
      <div class="box">1</div>
      <div class="box">2</div>
      <div class="box">3</div>
    </div>
    <div class="center">
      <div class="box">我居中了</div>
    </div>
  </body>
</html>
```
