内容取自Addy Osmani的文章：[DevTools Tips For Sublime Text Users](https://medium.com/google-developers/devtools-tips-for-sublime-text-users-cdd559ee80f8)

除了常见的Inspect和Profiling功能之外，Chrome DevTools还有编辑器的属性。你可以在DevTools里用快捷键来操作代码，也可以对编辑器格式进行设置，还可以为DevTools换上你自己中意的UI主题。

## 快捷键
我们可以在Chrome DevTools的`Sources`面板中使用各种快捷键操作，就像使用Sublime Text一样。

+ 找文件：`ctrl/cmd + p`
+ 找方法定义：`ctrl/cmd+ shift + p`
+ 定位到某一行：`ctrl + G`，可以输入行号，也可以输入字符串
+ 多光标同时编辑：按住`cmd / alt`选中多处
+ 选择多个occurrence：选中一个单词，按`cmd/Alt + D`，敲几次D，就会选择几个
+ 跳至行首尾：按住`cmd`，加左右方向键
+ 跳至上一次编辑位置：`Alt -/+`

更多操作不细说，完整地快捷键列表的查看方式：`DeTools Setting Menu -> Shortcuts`

![](https://cdn-images-1.medium.com/max/1200/1*ruU4iOfl63bDdOcHf0t6Hg.png)

## 编辑器设置

可以设置DevTools Sources编辑器的一些行为，比如代码缩进、括号匹配、代码智能感知、显示空白字符等等。

设置方法：`DeTools Setting Menu -> Settings -> General`

![](https://cdn-images-1.medium.com/max/1200/1*kNSTfEe7h8FJUgJ8eFd6bA.png)

## 主题
跟Sublime一样，你还可以为DevTools设置自己喜欢的主题。目前有这两个主题可供选择：

- [zerodarkmatrix](https://github.com/mauricecruz/chrome-devtools-zerodarkmatrix-theme)
- [greybeard](https://github.com/xero/greybeard-devtools)

安装方式请参考上面主题的Github Repo README文档。

