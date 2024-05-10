---
title: Linux 多视窗管理程序
categories: Linux
version: 1.1
---



### 

```bash
# 新建一个名为 session 的会话
screen -S <session>
```

### list
```bash
# 查看所有会话
screen -ls
```

### return

```bash
# 回到 session 会话
screen -r <session>
```

### keep and exit

```bash
Ctrl + A + D
```

### force detele

```bash
screen -X -S <session> quit
```

