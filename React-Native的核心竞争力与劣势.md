# React-Native核心竞争力

## 原生打包

* 打包优化
* 不依赖平台的webview性能（Hybrid依赖）
* 完全可控，无第三方打包依赖（不需要依赖类似codova）

## 虚拟DOM

> DOM是性能瓶颈

例如只需要将需要刷新的DOM节点映射到真实DOM树上即可

## 高性能的 JsBridge

* IOS： 使用JavaScriptCore做js解析
* Android : 通过jni层 C/C++实现高性能通信机制
* 不只是js与原生语言的互调

> 不支持4.1以下的原因:使用了Android api 16的渲染API



## 保留平台特性

* 官方UI保持平台特性
* 根据不同平台原生UI与原生，模块进行扩展
* 第三方库引入与管理



## FlexBox

* 与像素无关，适合移动端屏幕兼容

* 弹性布局

* 自适应

   
# 缺点
1. Android平台打包体积过大（bundle过大，.so库大）
2. 目前没有1.0 release，难免会有坑（官方文档，github中的issue）
3. 生态不够完善，很多组件需要自己桥接
4. react-native本身不兼容web端(有第三方扩展框架 react-web，携程moles)
5. 页面降级问题
