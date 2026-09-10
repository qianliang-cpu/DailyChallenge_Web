# Day_9 · 条件判断 if/else

> 预计耗时：20~30 分钟
> 让程序"会判断"：满足条件做一件事，否则做另一件事。

## 今日知识点

- `if (条件) { ... }` 满足才执行
- `else { ... }` 不满足时执行
- `else if` 多个分支
- 比较：`>` `<` `>=` `<=` `===`（等于）`!==`（不等于）

## 先学（教程）

- 菜鸟教程 JS（看"JS 条件语句"）：https://www.runoob.com/js/js-if-else.html
- MDN·条件判断：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/conditionals
- B站视频（黑马程序员，看讲"if/else 条件判断"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

> 从今天起，我们改用"写 `.js` 文件 + `node 文件名.js`"的方式运行代码（比控制台更正规，代码能保存、复用）。

新建 `day9.js`，用 VS Code 写，然后在终端里 `node day9.js` 运行（Day_0 已装好 Node）：

1. 判断成年：
   ```javascript
   let age = 18;
   if (age >= 18) {
     console.log("成年");
   } else {
     console.log("未成年");
   }
   ```
2. 分数评级：≥90 输出"优秀"、≥60 输出"及格"、否则"不及格"（用 `else if`）
3. 把 `age` 改成 15，再运行一遍，观察输出变化

## 完成标准

- [ ] 能写出 if/else 判断成年
- [ ] 能写出多分支分数评级
- [ ] 知道 `===` 和 `=` 的区别（一个是比较，一个是赋值）

**提交方式**：把 `day9.js` 代码 + 运行结果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
let age = 18;
if (age >= 18) {
  console.log("成年");
} else {
  console.log("未成年");
}

let score = 75;
if (score >= 90) {
  console.log("优秀");
} else if (score >= 60) {
  console.log("及格");
} else {
  console.log("不及格");
}
```
