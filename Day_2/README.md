# Day_2 · HTML 表单与输入控件

> 预计耗时：20~30 分钟
> 网页要能"填"：登录、注册、搜索都靠表单。今天认识最常用的输入控件。

## 今日知识点

- 表单容器 `<form>`
- 输入框 `<input type="text">`、密码 `type="password"`、单选 `type="radio"`、多选 `type="checkbox"`
- 按钮 `<button>`、下拉框 `<select>` + `<option>`、多行文本 `<textarea>`

## 先学（教程）

- 菜鸟教程 HTML（看"HTML 表单"）：https://www.runoob.com/html/html-forms.html
- MDN·你的第一个表单：https://developer.mozilla.org/zh-CN/docs/Learn/Forms/Your_first_form
- B站视频（黑马程序员，看讲"表单、input/select/textarea"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

新建 `signup.html`，做一个简单的**报名表单**，包含：

1. 姓名（text）、密码（password）
2. 性别（radio 两个，`name` 相同才能单选）
3. 意向方向（select 下拉：前端 / 后端）
4. 一个提交按钮（button）

> 提示：`name` 属性是给输入框"起名字"，表单提交时用来区分不同字段（比如 `name="gender"` 表示这是性别那一项）。

## 完成标准

- [ ] 表单能显示并填写
- [ ] radio 能单选
- [ ] 用了 input / select / button

**提交方式**：把 `signup.html` 代码贴在当日工单评论里。

## 参考解答（先做再看）

```html
<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8">
    <title>报名</title>
  </head>
  <body>
    <form>
      <p>姓名：<input type="text" name="name"></p>
      <p>密码：<input type="password" name="pwd"></p>
      <p>性别：
        <label><input type="radio" name="gender" value="男">男</label>
        <label><input type="radio" name="gender" value="女">女</label>
      </p>
      <p>方向：
        <select name="direction">
          <option value="frontend">前端</option>
          <option value="backend">后端</option>
        </select>
      </p>
      <button type="submit">提交</button>
    </form>
  </body>
</html>
```
