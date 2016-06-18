# page-init
前端页面渲染的工具库，ajax页面的渲染框架

## 相关介绍

主要流程：

1. 解析URL参数
2. 载入渲染配置
3. 渲染指定配置

page提供什么功能
用于支持使用ajax渲染的页面，目标就是抽离出这部分不变的工作，让用户通过提供页面数据来完成页面的渲染
* 在这里“页面数据”指的是渲染页面需要的json数据和相关的时间监听器

需要什么数据？
js方面：
* 页面需要的json数据以及对应的渲染模块
* 事件监听器
html方面：
* 渲染的模版

数据氛围监听器数据和渲染数据

具体需求：
* 渲染数据可以指定渲染策略，例如可以在页面加载完毕就渲染或者由用户在运行期间手动渲染
* 渲染数据中获取数据部分可以填函数或者对象，如果是对象，则当作ajax对象处理，如果是函数则无参数的调用这个函数获取结果
