---
title: 安卓终端常用命令
categories: Android
version: 13
---

## CPU

### Basic info

```bash
cat /proc/cpuinfo
```

#### Frequency

```bash
cat /sys/devices/system/cpu/cpu0/cpufreq/cpuinfo_max_freq
cat /sys/devices/system/cpu/cpu0/cpufreq/cpuinfo_min_freq
```

## System

### Props

```bash
getprop ro.product.brand
getprop ro.product.model
```

