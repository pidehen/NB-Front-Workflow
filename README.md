# 前端开发工作流

## 为什么要基于工作流
开发大中型前端项目，需遵循一定的规范，合理架构项目，运用工程化解决效率问题，避免重复劳动。

## 开发前端项目遇到哪些功能和开发中需要反复进行哪些操作
在开发中都会遇到 **DOM操作、数据请求、移动端适配、移动端Tap事件、路由分发、模板渲染** 等功能；

在编码过程中都需反复进行 **清扫目录、编译ES6/7、压缩/混淆、雪碧图、前缀CSS** 等操作；
现在就是要基于这个目的进行工作流构建，旨在提高前端开发效率。

## 工作流技术选型
* NB-Element.js + NB-AJAX.js + NB-MobileAdapter.js + NB-TapClick.js
* NB-Class.js(面向对象编程)
* NB-Router.js(路由分发)
* NB-Tpl.js(模板引擎)
* NB-MVC.js(MVC)
* NB-Package.js(模块化管理)
* NPM + 构建工具库

## NB-Element.js
进行元素获取、删除、替换、插入、修改样式和属性、特定属性和样式修改、动画

## NB-AJAX.js
通过传入请求头、请求地址、请求结构向远程服务端进行数据请求

## NB-MobileAdapter.js
移动端适配，一套代码适应不同分辨率的机型
其实就是先得出设备像素比，然后得到缩放，设置布局视口=理想市口，
在iphone中通过设置initial-scale=scale，android中通过设置initial-scale=1
然后设置根元素的font-size为当前屏幕尺寸 / 10，rem就是根据屏幕进行适配
