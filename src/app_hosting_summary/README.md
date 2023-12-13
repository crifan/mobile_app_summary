# APP托管总结

在发布到其他app托管平台期间，会涉及到给对于页面的命名


## 项目发布时页面命名规则

比如要将一个项目发布到`fir.im`时，给页面的短写的名字，命令，就和项目起包名，很类似。

建议`fir.im`中路径命名规则为：**项目名+平台+环境**

> Android：https://fir.im/XxxYyyiOS
> 
> iOS： https://fir.im/XxxYyyAndroid


比如：

* 项目名：驼峰法命名（camel casing）
  * Xxx
* 平台：iOS或Android等
* 环境：
  * 开发版=`dev`
  * 测试版=`test`=`tst`
  * 正式版
    * `production`=`prd`
    * `release`=`rls`

