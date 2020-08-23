## HTMl

### HTML语法

- 合法元素
  - Element 元素
  - Text 文本
  - Comment 注释
  - DocumentType <!Doctype html>
  - Processinglnstruction <?a 1?>
  - CDATA <![CDATA[ ]]!>
- 字符引用
  - &#161 ...
  - \&amp; &
  - \&lt; < \&gt; >
  - \&quot; "

## 浏览器API

### DOM API
- Node
  - Element 元素节点
   - HTMLElelement
   - SVGElement
  - Document 文档根节点
  - CharacterData 字符数据
  - DocumentFragment 文档片段
  - DocumentType 文档类型
- 导航类操作
  - Node
    - parentNode
    - childNodes
    - firstChild
    - lastChild
    - nextSibling
    - previousSibling
  - Element
    - parentElement
    - children
    - firstElementChild
    - lastElementChild
    - nextElementSibling
    - previousElementSibling
- 修改操作
  - appendChild
  - insertBefore
  - removeChild
  - replaceChild
- 高级操作
  - compareDocumentPosition 比较两个节点中的关系
  - contains
  - isEqualNode 检查两个节点是否完全相同
  - isSameNode  检查两个节点是否是同一节点
  - cloneNode 复制节点

### 事件 API
- 事件的冒泡和捕获

### Range API
- 创建range
  - var range = new Range();
  - range.setStart(element, 9);
  - range.setEnd(element, 4);
  - var range = document.getSelection().getRangeAt(0)
- other
  - range.setStartBefore
  - range.setEndBefore
  - range.setStartAfter
  - range.setEndAfter
  - range.selectNode
  - range.selectNodeContents
- rang操作
  - var fragment = range.extractContents()
  - range.insertNode(document.createTextNode('aaa'));
  
### CSSOM

- document.styleSheets
  - rules
    - document.styleSheets[0].cssRules
    - document.styleSheets[0].insertRule("P{color: bloack}", 0)
    -document.styleSheets[0].removeRule
    