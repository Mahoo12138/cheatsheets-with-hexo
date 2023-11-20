---
title: 基于Python一个交互式笔记本
categories: Python
version: 4.6.3
---

##  基本配置

### 安装

```bash
pip install juypter
```

### 生成配置文件

```bash
jupyter notebook --generate-config
```

### 启动

```shell
jupyter notebook
```

## 主题配置

### 安装主题

```bash
pip install jupyterthemes
```

### 更新主题

```bash
pip install --upgrade jupyterthemes
```

### 主题列表

```bash
jt -l
```

### 设置主题

```bash
# 详细配置查看 $jt -h
jt -t <name-of-theme>
#  -T, --toolbar         make toolbar visible
```

## 插件配置

### 插件安装

```bash
pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install
```

