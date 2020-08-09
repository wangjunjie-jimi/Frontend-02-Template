## CSS

### 总体结构

- @charset
- @import
- rules
  - @media
  - @page
  - rule

### @规则

- @charset
- @import
- @media
- @oage
- @counter-style
- @keyframes
- @fontface
- @supports
- @namespace

### css规则

- 选择器

- key
  - 属性
  - 变量
- value

### css选择器语法
- 简单选择器
  - \*
  - div svg|a 元素
  - .cls 类
  - #id id
  - [attr=value] 属性
  - :hover 伪类
  - ::before 伪元素

- 复合选择器
  - <简单选择器><简单选择器><简单选择器>
  - \*/div 必须写在最前面
- 复杂选择器
  - <复合选择器><sp><复合选择器>
  - <复合选择器>">"<复合选择器>
  - <复合选择器>"~"<复合选择器>
  - <复合选择器>"+"<复合选择器>
  - <复合选择器>"||"<复合选择器>

### 伪类
- 链接/行为
  - :any-link 匹配任何的超链接
  - :link :visited 未访问和已访问的链接
  - :hover 
  - :active 
  - :focus
  - :target 链接到当前目标

- 树结构
  - :empty
  - :nth-child()
  - :nth-last-child()
  - :first-child :last-child :only-child

- 逻辑型
  - :not 主要
  - :where :has

### 伪元素
- 增加元素
  - ::before
  - ::after
- 不增加元素，把元素包裹
  - ::first-line 针对**排版**以后的第一行
  - ::first-letter