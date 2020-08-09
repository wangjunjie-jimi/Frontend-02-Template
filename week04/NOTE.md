## 浏览器工作原理

### 浏览器

1. 浏览器基础渲染流程

url(http 请求) ---> html(parse 编译) --> DOM(css 计算) --> DOM with css(layout 布局/排版) --> DOM with position(render 渲染) --> Bitmap

2. ISO-OIS 七层网络模型

3. TCP与IP
 - 流               
 - 端口
 - require('net')
 - 包
 - IP地址
 - libnet(构造IP包并发送)/libpcap(抓取ip包)
4. HTTP
 - request
 - response
 - 每一个request对应一个response 
 
### 状态机

1. 有限状态机
   - 每个状态都是一个机器
   - 每一个机器知道下一个状态

4) 使用有限状态机处理字符串
   - a.b = c √ 左手表达式
   - a + b = c × 右手表达式

