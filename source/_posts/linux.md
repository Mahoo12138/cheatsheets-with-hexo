---
title: Linux 基础命令
categories: Linux
version: all
top: true
---

### get owner of file

```bash
USER=$(stat -c '%U' /path/to/your/file)
GROUP=$(stat -c '%G' /path/to/your/file)
```

%u     user ID of owner
%U     user name of owner
%g     group ID of owner
%G     group name of owner