---
title: 进程管理软件 PM2
categories: Linux
version: 5.2.2
---

### npm start

```bash
pm2 start npm --watch --name <taskname> -- run <scriptname>
```

### common script

```bash
pm2 start dist/main.js --name <taskname>
```

