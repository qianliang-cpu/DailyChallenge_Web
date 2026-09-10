# Day_10 · 循环 for / while

> 预计耗时：20~30 分钟
> 让程序"会重复"：把同一件事做很多遍，不用复制粘贴。

## 今日知识点

- `for (let i = 0; i < 5; i++) { ... }` 重复执行固定次数
- `while (条件) { ... }` 满足条件就一直执行
- 循环里用 `i` 计数

## 先学（教程）

- 菜鸟教程 JS（看"JS 循环"）：https://www.runoob.com/js/js-loop.html
- MDN·循环：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Looping_code
- B站视频（黑马程序员，看讲"for/while 循环"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

新建 `day10.js`：

1. 用 `for` 打印 1 到 5：
   ```javascript
   for (let i = 1; i <= 5; i++) {
     console.log(i);
   }
   ```
2. 用 `for` 打印 1 到 10 里的**偶数**（提示：`if (i % 2 === 0)`）
3. 用 `while` 从 10 倒数到 1

## 完成标准

- [ ] for 循环打印 1~5
- [ ] 能筛出偶数
- [ ] while 循环能倒数

**提交方式**：把 `day10.js` 代码 + 运行结果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}

for (let i = 1; i <= 10; i++) {
  if (i % 2 === 0) {
    console.log(i);   // 2 4 6 8 10
  }
}

let n = 10;
while (n >= 1) {
  console.log(n);
  n--;
}
```
