# Day_11 · 函数：把代码装进"盒子"反复用

> 预计耗时：20~30 分钟
> 把一段代码打包，起个名字，之后随时调用。函数是写程序的必备技能。

## 今日知识点

- 定义：`function 名字(参数) { ... return 结果; }`
- 调用：`名字(参数)`
- `return` 返回结果，没有就返回 `undefined`

## 先学（教程）

- 菜鸟教程 JS（看"JS 函数"）：https://www.runoob.com/js/js-functions.html
- MDN·函数：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Functions
- B站视频（黑马程序员，看讲"函数定义、参数、返回值"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

新建 `day11.js`：

1. 加法函数：
   ```javascript
   function add(a, b) {
     return a + b;
   }
   console.log(add(3, 5));   // 8
   ```
2. 写一个 `isAdult(age)`，年龄 ≥18 返回 `true`，否则 `false`，并调用打印
3. 写一个 `greet(name)`，返回 `"你好，" + name`

## 完成标准

- [ ] 会用参数和 return
- [ ] 能调用自己写的函数
- [ ] 能说出 return 和 console.log 的区别

**提交方式**：把 `day11.js` 代码 + 运行结果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
function add(a, b) {
  return a + b;
}
console.log(add(3, 5));        // 8

function isAdult(age) {
  return age >= 18;
}
console.log(isAdult(20));      // true
console.log(isAdult(15));      // false

function greet(name) {
  return "你好，" + name;
}
console.log(greet("张三"));
```
