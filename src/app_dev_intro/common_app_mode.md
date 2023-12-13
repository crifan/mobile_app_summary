# 常见APP模式

正如前面的介绍，一般项目涉及到的APP模式，可以简化立即为有三种：

* 纯Web=纯Web页面适配移动端
* Web App=移动端混合APP
* Native App=纯原生移动端APP

而其中的 纯Web的，指的是一套Web页面，完全适配移动端浏览器，所以还是属于基于浏览器的页面，不算传统意义上的移动端的APP，所以不做详细解释。

接下来主要解释：混合式的Web App和纯的Native原生APP。

## Web App对比Native App

详细解释之前，对于典型的Web的APP和原生的Native的APP进行一个简单的对比：

| Native App | Web App | 说明 |
| ---------- | ------- | --- |
| 偏交互 | 偏浏览 | 交互指复杂操作，输入/选择什么的 |
| 已稳定 | 试错中 | H5页面用来做低成本验证很好 |
| 访问硬件 |信息展示 | 指手机里的各种传感器什么的 |
| 核心功能 | 周边辅助 | 把工作量多投在刀刃上 |

## 原生Native

原生的APP，概念上其实很简答， 就是指的是：

* iOS平台：典型的指的是，在Mac的Xcode下，用纯的之前的`Objective-C`或最新的`Swift`的代码开发和调试，最终生成的原生的iOS的ipa文件
* Android：在`Mac`/`Windows`系统中，用之前的`Eclipse+ADT`或最新的`Android Studio`工具，写之前的`Java`或最新的`Kotlin`代码，去开发调试出来的Android原生的apk文件

## 混合APP

关于混合APP开发，往往指的是：用一套框架或技术，最终得到的app。

### H5+原生的壳

其中，用原生的app写个基本的启动界面，加上一个WebView，然后用webview去加载所有的app的内容，即一堆的HTML+CSS+JS，从而实现app的效果。

所以，就分成两部分：

* H5页面=Webview页面
* 原生的壳=原生代码(iOS/Android)去写对应的app客户端
  * 可能还包括一些其他相关的基本功能：
    * 启动页面
    * 自动保存密码
      * 用于实现自动登录
    * 消息推送
      * 纯Web页面无法（很难）做到消息推送，只能靠原生

如此，H5+原生的壳，就实现了一个移动端的APP，如果效果做的还可以，基本上可以以假乱真，看起来和原生的APP没多大区别。

对于的这类移动端的Web页面的设计，也有专门的逻辑和注意事项，比如：

[Mobile Web Development - Web developer guides | MDN](https://developer.mozilla.org/en-US/docs/Web/Guide/Mobile)

### 混合APP框架

另外一种实现一般所谓的混合APP的做法就是：使用某个混合APP框架去实现

而混合式APP框架，又可以分为两类：

* 传统混合APP框架
* 新出的一些特殊的框架

下面分别来介绍。

#### 传统混合APP框架

传统的框架，有很多，其中一些比较出名的有：

##### cordova(旧称PhoneGap)

之前叫PhoneGap，后被Adobe收购了改名为cordova。

主页：[Apache Cordova](https://cordova.apache.org)

##### ionic

还有一个混合APP框架`ionic`，好像用的也不少

主页：[Build Amazing Native Apps and Progressive Web Apps with Ionic Framework and Angular](https://ionicframework.com)

#### 新出现的基于JavaScript的框架

后来又出现一些，从广义上也可以被称为混合式APP框架的：

##### React Native

`React Native`=`RN`

Facebook出的，可以用一套`React Native`框架，写JS代码，最终生成iOS和Android两端的App。

性能总体上比纯Web要好。

主页：[React Native · A framework for building native apps using React](https://facebook.github.io/react-native/)

##### weex

阿里的出的，目标是支持一套代码，生成iOS、Android和Web端的程序。

常常被拿来和RN对比。

目前流行度好像一般。

主页：[Weex](https://weex.apache.org)

##### HBuilder

还有个叫做`HBuilder`，好像不是很流行，但是之前简单尝试过，没具体折腾。

好像也可以生成APP，但是感觉是一个官网的原生的APP壳，加上内部的Webview的效果。

也算作其中一个框架吧，虽然可能是从功能上来说是比较弱的。

主页：[DCloud - HBuilder、5+、mui、流应用、HTML5专家](http://www.dcloud.io)
