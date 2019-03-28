# 课后总结

### Vue.component 缺点

- 全局定义：强制要求每个 component 中的命名不得重复
- 字符串模板：缺乏语法高亮，在 HTML 有多行的时候，需要用到丑陋的'\'
- 不支持CSS：意味着当 HTML 和 JavaScript 组件化时，CSS 明显被遗漏
- 没有构建步骤：限制只能使用 HTML 和 ES5 JavaScript，而不能使用预处理器，如 Pug(formerly Jade) 和 Bable
