---
layout: default
title: Synchronous or Asynchronous and callback~
---
　　
昨天下午纠结了一下午的同步异步回调，单线程多线程的问题，以及Node.js的单线程异步的问题。看了网上很多资料，中文的英文的，都是用一些有的没的例子讲得不清不楚，完全把异步和同步割裂来看待了。甚至包括对于callback的理解也是略有问题。

一开始我以为callback就是指的如下这种定义
>A callback is a function that is passed as an argument to another function and is executed after its parent function has completed. The special thing about a callback is that functions that appear after the "parent" can execute before the callback executes. Another important thing to know is how to properly pass the callback. 

但是这种定义太肤浅了，不一定是要以一种argument的形式来使用。如果你明确的知道自己要用什么函数来回调的话，你是可以来直接调用的，但是比较常见用这种函数作为parameter的形式，因为有时候你call过去的模块只是给你提供了接口，那个模块也不事先知道你要用什么样的callback函数，所以直接作为参数传过去是科学的。

昨天想半天Node.js的所谓单线程异步是咋实现的，大家都在讲什么setTimeOut各种绕得飞。好人小王说，对于我写的.js文件程序当然是单线程，但是对于Node.js整体来说，它还有别的线程在辅助执行。

一想到上学期为了进程和线程的抽象概念半天理解不了就是感到好笑，现在已经逐渐习惯这种抽象的方式了。

* file———>storage
* address space ———>memory
* process&thread ———>CPU

昨天下午还研究了下，用Node.js开发了个异常简单的web应用，发现挺有趣的。还用npm下了个package。试用了下visual studio code，超级好用呢，快捷键的设置也是real跟别人不同。

一想到今天又要学习typescript并且要把JavaScript再次学习一边，我这张老脸就泛起了微笑。。。还有GO语言什么的，每学期都被新的内容虐，感觉技能树都要长岔了。。。😊





