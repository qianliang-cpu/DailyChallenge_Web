# Day_7 · JavaScript 入门：变量与数据类型

> 预计耗时：20~30 分钟
> 进入第二周。JavaScript（JS）是网页的"大脑"，负责交互。今天先学会在浏览器里运行 JS，认识变量和数据类型。

## 今日知识点

- 在浏览器里运行 JS：打开任意网页 → F12 → 控制台（Console），直接输入代码回车
- 变量：`let` 声明变量、`const` 声明常量
- 数据类型：`string`（字符串）、`number`（数字）、`boolean`（true/false）
- 输出：`console.log(...)`

## 先学（教程）

- 菜鸟教程 JS（看"JS 简介""JS 输出""JS 变量"）：https://www.runoob.com/js/js-tutorial.html
- MDN·JS 第一步：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps
- B站视频（黑马程序员，看讲"变量、常量、数据类型"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

打开浏览器 F12 控制台，逐行输入并回车：

1. `let name = "张三";` 回车，再输入 `console.log(name);`
2. `let age = 18;` 再 `console.log(age);`
3. `const PI = 3.14;` 再 `console.log(PI);`
4. `let isStudent = true;` 再 `console.log(isStudent);`
5. 试试 `typeof name` 和 `typeof age`，看看它们是什么类型

> 每次重新打开控制台，之前定义的变量会清空。
> 注意：`let` 不能重复声明同名变量，若报 `has already been declared`，刷新控制台再继续。

## 完成标准

- [ ] 能在控制台输出字符串、数字、布尔值
- [ ] 会用 `typeof` 查看类型
- [ ] 能说出 `let` 和 `const` 的区别（const 不能重新赋值）

**提交方式**：把控制台的**截图**（能看到你输入的代码和输出）贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
let name = "张三";
console.log(name);        // 张三

let age = 18;
console.log(age);         // 18

const PI = 3.14;
console.log(PI);          // 3.14

let isStudent = true;
console.log(isStudent);   // true

typeof name;              // "string"
typeof age;               // "number"
```
