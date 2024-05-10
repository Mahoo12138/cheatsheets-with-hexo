---
title: Windows 快捷使用清单
categories: System
version: 1904
---

### 端口占用

```shell
netstat -ano              # 查看所有端口占用
```

```shell
netstat -ano|findstr 3306 # 查看具体端口占用
tasklist|findstr 12138    # 根据PID查看占用程序
taskkill /f /pid 12138    # 根据PID杀死占用程序
```

### IP 扫描

```powershell
arp -a
```

### DNS 相关

```bash
ipconfig /flushdns      # 清除 DNS 缓存
ipconfig /displaydns    # 查看清除记录
```

### 文件树

```bash
# 命令提示
tree /?

# 显示当前目录下的目录树(不显示文件)
tree

# 递归显示目录结构(显示文件，常用于项目说明)
tree /F
 
# 将显示的内容重定向到txt
tree > info.txt
tree /F > info.txt
```

### 目录

+ `c:\Users\Mahoo12138\AppData\Roaming\*`

## Powershell

### File 

```powershell
# create a text file
New-Item mahoo.txt
```

