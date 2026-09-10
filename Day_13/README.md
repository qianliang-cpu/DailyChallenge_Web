# Day_13 · 对象 Object 与 JSON（第二周小测）

> 预计耗时：20~30 分钟
> 对象把一组相关的数据打包在一起（比如一个人的姓名、年龄、爱好）。JSON 是前后端传数据的通用格式。今天认识它们。

## 今日知识点

- 对象：`{ 键: 值, 键: 值 }`，用 `对象.键` 取值
- JSON：本质是"字符串形式的对象"，常用于接口传数据
- `JSON.stringify(对象)` 转字符串；`JSON.parse(字符串)` 转回对象

## 先学（教程）

- 菜鸟教程 JS（看"JS 对象"和"JS JSON"）：https://www.runoob.com/js/js-json.html
- MDN·JSON：https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Objects/JSON
- B站视频（黑马程序员，看讲"对象、JSON"的几集，选看）：https://www.bilibili.com/video/BV1Y84y1L7Nn/

## 任务（后做）

新建 `day13.js`：

1. 建一个对象：
   ```javascript
   let person = {
     name: "张三",
     age: 18,
     hobbies: ["代码", "篮球"]
   };
   console.log(person.name);
   console.log(person.hobbies[0]);
   ```
2. 用 `JSON.stringify(person)` 转成字符串，打印看看长什么样
3. 用 `JSON.parse` 把这段字符串转回对象，再打印 `.age`

## 完成标准

- [ ] 会用 `对象.键` 取值
- [ ] 会 JSON 字符串和对象的互相转换
- [ ] 能说出对象和 JSON 字符串的区别

**提交方式**：把 `day13.js` 代码 + 运行结果截图，贴在当日工单评论里。

## 参考解答（先做再看）

```javascript
let person = {
  name: "张三",
  age: 18,
  hobbies: ["代码", "篮球"]
};
console.log(person.name);      // 张三
console.log(person.hobbies[0]); // 代码

const json = JSON.stringify(person);
console.log(json);
// {"name":"张三","age":18,"hobbies":["代码","篮球"]}

const obj = JSON.parse(json);
console.log(obj.age);          // 18
```

> 恭喜！两周的基础都走完了。下一步进入 DOM 操作、事件、异步和 Vue，请期待后面的课程。
