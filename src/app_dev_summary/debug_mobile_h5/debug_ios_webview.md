# 调试iOS的Webview

把iOS设备，比如iPhone手机连接到Mac上之后:

![iPhone用数据线连接到Mac上](../../assets/img/iphone_usb_cable_connect_mac.png)

打开Mac中的Safari浏览器，在已经开启开发模式（显示出开发菜单）后，可以在：

`开发` -> `xxx iPhone` -> 选择对应的页面：

![Mac中Safari开发选择iPhone的页面](../../assets/img/mac_safari_dev_choose_iphone_page.png)

即可去调试手机移动端中的（WebKit内核的）页面。鼠标移动到对应的html的元素上之后，手机端的页面的对应部分即可实时显示出背景色了：

![Mac中鼠标移动后iPhone中元素显示背景色](../../assets/img/mac_mouse_move_iphone_html_background.jpg)

## Safari中显示`开发`菜单

`Safari` -> `配置` -> 勾选`在菜单中显示"开发"菜单` -> 菜单中就可以看到`开发`菜单了：

![Mac中Safari中显示开发菜单](../../assets/img/mac_safari_show_dev_menu.png)
