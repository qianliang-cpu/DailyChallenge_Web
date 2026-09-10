# Day_6 · 响应式基础 + 看懂一个 AI 页面（第一周小测）

> 预计耗时：25~30 分钟
> 手机屏幕窄、电脑宽，页面要"自适应"。今天学媒体查询，然后**不手写**，试着看懂一段 AI 生成的页面。

## 今日知识点

- 媒体查询：`@media (min-width: 768px) { ... }` —— 屏幕 ≥768px（桌面）时套用；`max-width` 则是"≤768px（手机）时套用"
- viewport：`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- 第一周目标：**不要求独立手写，能看懂 AI 生成的 HTML/CSS 即可**

## 先学（教程）

- 菜鸟教程 CSS 响应式：https://www.runoob.com/css/css-rwd-viewport.html
- MDN·响应式设计入门：https://developer.mozilla.org/zh-CN/docs/Learn/CSS/CSS_layout/Responsive_Design
- B站视频（黑马程序员，看讲"视口、媒体查询、响应式"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

1. 给一个容器加 `viewport` meta，卡片默认一列，`@media (min-width: 768px)` 时排成一行（参考解答可看，今天看懂为主）
2. **重点任务**：用 AI 生成一个"个人主页"页面（HTML+CSS），然后**逐块说出**它是怎么实现的：
   - 导航栏是怎么两端对齐的？
   - 卡片区是用什么布局排成一行的？
   - 哪个选择器、哪些属性在起作用？
   把你说出来的理解写在工单评论里（不用你写代码，能讲明白就行）

## 完成标准

- [ ] 加了 viewport，媒体查询能切换布局
- [ ] 能说清楚 AI 页面里至少 3 处用到的 CSS 知识点

**提交方式**：把响应式页面的截图 + 你对 AI 页面的**文字理解**（50 字以上），贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>响应式</title>
    <style>
      .cards {
        display: flex;
        flex-direction: column;   /* 手机：一列 */
        gap: 20px;
      }
      .card {
        border: 1px solid #ddd;
        border-radius: 8px;
        padding: 20px;
      }
      @media (min-width: 768px) {  /* 桌面：一行 */
        .cards { flex-direction: row; }
        .card { flex: 1; }
      }
    </style>
  </head>
  <body>
    <div class="cards">
      <div class="card">卡片 1</div>
      <div class="card">卡片 2</div>
      <div class="card">卡片 3</div>
    </div>
  </body>
</html>
```
