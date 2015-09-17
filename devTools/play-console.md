Chrome的Console面板是一个REPL(read-eval-print loop，交互式解释器)。

## 简介
它是一个常用工具函数的集合，Chrome把这些函数暴露在Console接口里。你可以在Console面板里使用这些函数来：

- 选取页面中的DOM元素（类似于jQuery）
- 执行ECMAScript（调用Chrome的V8来执行）
- 监控DOM事件
- Profiling

PS: 以上行为都只能在Console面板里执行，你无法在页面的JavaScript中执行以上行为。

## 内容

官方文档：[Command Line API Reference](https://developers.google.com/web/tools/javascript/command-line/command-line-reference)

### DOM操作

### monitor()

### profile()

## 题外话

Chrome Console十分强大，提供了太多的接口。有些接口由于考虑不周而留下了安全隐患，被不法黑客利用。

Facebook就曾深受其害，不得已而在Facebook页面上禁用了Chrome Console。

故事详细：[How does Facebook disable the Chrome DevTools](https://github.com/simongong/js-stackoverflow-highest-votes/blob/master/questions11-20/how-facebook-disables-chrome-console.md)