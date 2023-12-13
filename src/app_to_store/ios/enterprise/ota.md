# OTA版

## 坑：打包OTA包时的设置的图片地址也要正确否则无法下载

iOS打包OTA的安装包时，即使只是图片有问题（而ipa没问题），也会导致无法正常下载和安装

详见：
[［已解决］企业版的iOS的app去In House打包和OTA发布后有时候无法下载和安装：无法下载应用 此时无法下载 完成 重试](http://www.crifan.com/ios_enterprise_inhouse_ota_cannot_download_this_application)

## 坑：打包OTA包时plist中的ipa文件或图片的地址中如果包含特殊字符也会导致无法正常下载

对于ipa或图片的文件地址中如果包含特殊不可见字符的话，也是会导致无法下载的。

详见：

[［已解决］企业版iOS的ipa通过OTA发布后还是无法下载和安装](https://www.crifan.com/enterprise_ios_ipa_ota_release_still_can_not_download_install/)
