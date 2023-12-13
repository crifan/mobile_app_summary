# APP相关项目常见模式

APP相关的项目的开发，目前常见有如下几种方案/模式：

## 纯Web模式

PC端：Web页面
手机端：（移动端）Web页面，页面适配手机/Pad等屏幕大小

方案：

* Web页面
  * JS框架：
    * jQuery
    * Agular JS
    * Vue.Js
    * React JS
  * UI框架
    * Bootstrap

## PC端Web+App混合模式

PC端：一套Web页面，适配PC端
移动端：一套Web页面，适配移动端 + APP端打包一个壳，内置Webview，加载显示web页面

方案：

* Web页面：
  * JS框架：
    * jQuery
    * Agular JS
    * Vue.Js
    * React JS
* APP端
  * iOS
    * 开发工具：Android Studio
      * 只是开发个壳，嵌入chrome的webview，用webview加载web页面
  * Android
    * 开发工具：（Mac）Xcode
      * 只是开发个壳，嵌入safari的UIWebView，用UIWebView加载web页面
        * 另外一种，虽然和Webview+原生的壳不同，但是也属于广义上的混合APP的模式：
        * React Native的混合模式
        * 用React Native写Javascript代码，一套代码
        * -> 生成iOS和Android的原生的app

## PC端Web + App端：原生APP

* Web页面
  * JS框架
    * `jQuery`
    * `Agular` JS
    * `Vue`.Js
    * `React` JS
* APP端
  * Android
    * 开发工具：`Android Studio`=`AS`
      * 开发完整的独立的app的完整功能
  * iOS
    * 开发工具：（Mac中的）Xcode
      * 开发完整的独立的app的完整功能
