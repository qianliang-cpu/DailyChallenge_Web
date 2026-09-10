# Day_12 · 数组方法 push / filter / map / forEach

> 预计耗时：20~30 分钟
> 数组是一串数据的列表。今天学 4 个最常用的数组方法，后续做项目全靠它们。

## 今日知识点

- `push(x)`：往数组末尾加一个
- `forEach(fn)`：遍历每个元素，挨个处理
- `map(fn)`：把每个元素变一下，得到新数组
- `filter(fn)`：筛出满足条件的元素

## 先学（教程）

- 菜鸟教程 JS（看"JS 数组"和"JS 数组方法"）：https://www.runoob.com/js/js-array-methods.html
- MDN·数组：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps/Arrays
- B站视频（黑马程序员，看讲"数组操作、forEach/map"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

新建 `day12.js`：

1. `let nums = [1, 2, 3];` 用 `push(4)` 再打印，看结果
2. 用 `forEach` 遍历 `[1, 2, 3, 4, 5]`，打印每个元素（写法：`[1,2,3,4,5].forEach(function(n){ console.log(n); })`）
3. 用 `map` 把 `[1, 2, 3]` 变成 `[2, 4, 6]`（每个乘 2，写法：`[1,2,3].map(function(n){ return n * 2; })`）
4. 用 `filter` 从 `[1, 2, 3, 4, 5, 6]` 里筛出偶数

## 完成标准

- [ ] 会用 push 加元素
- [ ] 会用 forEach / map / filter
- [ ] 能说出 map 和 forEach 的区别（map 返回新数组）

**提交方式**：把 `day12.js` 代码 + 运行结果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
let nums = [1, 2, 3];
nums.push(4);
console.log(nums);          // [1, 2, 3, 4]

[1, 2, 3, 4, 5].forEach(function (n) {
  console.log(n);
});

const doubled = [1, 2, 3].map(function (n) {
  return n * 2;
});
console.log(doubled);       // [2, 4, 6]

const even = [1, 2, 3, 4, 5, 6].filter(function (n) {
  return n % 2 === 0;
});
console.log(even);          // [2, 4, 6]
```

> 传给 forEach / map / filter 的那个 `function (n) { ... }` 叫"回调函数"，
> 数组会把它套在**每一个元素**上各执行一次。先按这种写法记，后面会学更简短的箭头函数写法。
