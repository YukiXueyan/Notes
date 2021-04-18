## Node.js基础知识

### 1.1 概述

#### 1.1.1 Node.js是什么

#### 1.1.2Node.js带来了什么

### 1.2Node.js配置开发

#### 1.2.1 Windows配置

#### 1.2.2 Linux配置

#### 1.2.3 Hello World

#### 1.2.4常见问题

### 1.3 异步编程

#### 1.3.1同步调用和异步调用

#### 1.3.2回调和异步调用

#### 1.3.3获取异步函数的执行结果

## 模块和NPM

### 2.1 什么是模块

#### 2.1.1模块的概念

模块分为原生模块和文件模块

#### 2.1.2 Node.js 如何处理模块

1. 原生模块的调用

   `var http = require('http');`加载模块

   `http.createServer(function (req, res){}).listen()`调用方法

2. 文件模块的调用

#### 2.1.3 Node.js 实现Web解析DNS·

#### 2.1.4 Node.js重构DNS解析网站

#### 2.1.5exports 和 module.exports

### 2.2 NPM简介

#### 2.2.1 NPM 和配置

#### 2.2.2 Express框架

#### 2.2.3jade模板

#### 2.2.4 forever模块

#### 2.2.5 [socket.io](http://socket.io)模块

#### 2.2.6request模块

#### 2.2.7 Formidable模块

#### 2.2.8 NPM模块开发指南

### 2.3 Node.js设计模式

#### 2.3.1 模块与类

#### 2.3.2 Node.js中的继承

#### 2.3.3单例模式

#### 2.3.4适配器模式

#### 2.3.5装饰模式

#### 2.3.6工厂模式