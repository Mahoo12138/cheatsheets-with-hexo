---
title: 安卓开发调试工具
categories: Android
version: 1.1
---

## adb

详细命令查看 Google 官方 Guide：https://developer.android.google.cn/studio/command-line/adb#issuingcommands

### 安装 App

```bash
# 覆盖安装
adb install <apk file> -r
# 安装到sdcard
adb install <apk file> -s
# 允许降级覆盖安装
adb install <apk file> -d
```

### 卸载 App

```bash
# -k 参数为是否保留数据和缓存
adb unstall -k <package-name>
```

### 清除应用数据与缓存

```bash
adb shell pm clear <package-name>
```

##### 文件传输

```bash
# 传输到手机
adb push C:\Users\Mahoo12138\Desktop\test.zip /storage/sdcard
```

```bash
# 传输到 PC
adb pull /system/priv-app/DeviceTest/DeviceTest.apk C:\Users\Administrator\Desktop\
```

### 远程连接 ADB

```bash
# 同一局域网下，连接数据线
adb tcpip 5555
# 拔除数据线
adb connect <device_ip_address>
```

### 查看IP地址

```bash
# interface name for example: wlan0
adb shell ifconfig <interface_name>
```


#### 网络代理

```bash
# 设置代理
adb shell settings put global http_proxy <ip:port>
# 关闭代理
adb shell settings put global http_proxy :0
```
