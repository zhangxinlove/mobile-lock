# mobile-lock
移动端手势密码组件

### demo演示
 [地址](http://tangzhirong.github.io/lock/example/demo.html)
 
使用方法
=======================
### 在html中引入css和js文件：
    
### 
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width,initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no"/>
        <title>移动端手势密码组件</title>
        <link rel="stylesheet" type="text/css" href="../src/lock.css">
    </head>
    <body>
    <script type="text/javascript" src="../src/lock.js"></script>
    </body>
    </html>
###  加入如下script脚本

###
    <script type="text/javascript">
        //获取设备屏幕宽度
        var screenWidth = window.screen.width;
        //构造专属于你的手势密码
        var yourLock = new lock({
            size:screenWidth,  //手势区大小由设备screen宽度决定
            title:"小米5s手势密码",  //设置组件头部标题
            panelSize:3  //设置手势区单边圆圈数，默认为3个
        });
        yourLock.renderDom();  //创建DOM结构
        yourLock.init();   //初始化组件
        yourLock.bindEvent();  //绑定事件
    </script>
