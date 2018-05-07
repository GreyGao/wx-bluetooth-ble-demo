# wx-bluetooth-ble-demo
微信小程序蓝牙模块demo，可对蓝牙4.0 支持BLE的设备进行配对连接。

请使用微信开发者工具进行调试.

核心代码只有pages/index/index.js和index.wxml两部分。

主要有以下几个关键步骤：
1. 载入页面时初始化蓝牙模块
2. 扫描可连接的设备
3. 在页面中渲染可连接设备的列表
4. 连接设备，获取设备的deviceId
5. 获取设备的对应Services值与characteristics值
6. 开启notify活动监听
7. 成功读写数据
8. 断开连接

目前尚未完善的部分：
1. 目前只在安卓平台进行了测试，iOS还未完善；
2. 对于各个环节连接失败的情况尚未做较好的提示和处理；
3. 对于services和characteristics的值都简单的默认取了数组第一个，不知道不同的设备是否有不同，可以按需注入；
4. 目前只针对BLE设备连接。

效果图如下：
![screenshot2](https://i.loli.net/2018/05/07/5af03da2318ca.png)
![screenshot1](https://i.loli.net/2018/05/07/5af03da2310c7.png)

