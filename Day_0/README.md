# Day_0 · 配置开发环境（VS Code + Node.js + 终端 + 浏览器）

> 预计耗时：20~30 分钟
> 前端一切从工具开始。今天装好编辑器 VS Code 和运行环境 Node.js，学会用终端，认识浏览器开发者工具。

## 今日知识点

- VS Code：写代码的编辑器，装几个常用插件
- Node.js：让你能在电脑上运行 JavaScript（第二周会用 `node` 命令跑脚本）
- 终端（命令行）：执行命令的地方，Windows 上是 PowerShell / CMD
- 浏览器开发者工具：按 F12 打开，前端调试全靠它

## 先学（教程）

- VS Code 官方文档·入门：https://code.visualstudio.com/docs
- MDN·浏览器开发者工具入门：https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/Tools_and_setup/What_are_browser_developer_tools
- B站视频（黑马程序员，看讲"软件下载、VSCode 使用"的几集，选看）：https://www.bilibili.com/video/BV14J4114768/

## 任务（后做）

1. 下载安装 VS Code：https://code.visualstudio.com/ ，一路下一步
2. 在 VS Code 扩展商店（左侧方块图标）搜索并安装四个插件：
   - **Live Server**（预览网页用，安装好之后可以通过在文件页点击鼠标右键选择“open with live server”的方式在浏览器实时观看你所写的静态网页）
   - **Chinese (Simplified)**（中文界面，可选）
   - **Prettier**（自动格式化代码）
   - **HTML CSS Support**
3. 下载安装 Node.js：https://nodejs.org/ （选 **LTS** 版本，一路下一步），
   装好后打开终端运行 `node --version`，能看到版本号即成功
4. 打开终端（Windows 按 `Win + R` 输入 `cmd` 回车），运行 `ver` 或 `dir`，看看能输出什么
5. 随便打开一个网页，按 F12，认识"元素"和"控制台"两个面板

> 小贴士：终端里输入命令后回车才会执行；VS Code 底部也能打开内置终端。

## 完成标准

- [ ] VS Code 安装成功，四个插件装好
- [ ] `node --version` 能输出版本号
- [ ] 终端能运行命令
- [ ] 能按 F12 打开开发者工具

**提交方式**：把 VS Code 打开（含插件栏）+ 开发者工具的**截图**贴在当日工单评论里。
