---
title: C中各数据类型占字节数
categories: Programming
version: 1.1
---



Numerical type sizes in C (bits)

| Platforms  \   Types     | char | short | int  | size_t | ssize_t | long | long long | void * | off_t | float | double |
| :----------------------- | :--: | :---: | :--: | :----: | :-----: | :--: | :-------: | :----: | :---: | :---: | :----: |
| Win32, gcc nuwen 7.2     |  8   |  16   |  32  |   32   |   32    |  32  |    64     |   32   |  32   |  32   |   64   |
| Win32, gcc nuwen 7.2 LFF |  8   |  16   |  32  |   32   |   32    |  32  |    64     |   32   |  32   |  32   |   64   |
| Win32, MSVC              |  8   |  16   |  32  |   32   |    -    |  32  |    64     |   32   |  32   |  32   |   64   |
| Linux32, gcc             |  8   |  16   |  32  |   32   |   32    |  32  |    64     |   32   |  32   |  32   |   64   |
| Linux32, gcc LFF         |  8   |  16   |  32  |   32   |   32    |  32  |    64     |   32   |  64   |  32   |   64   |
| Win64, gcc mingw64       |  8   |  16   |  32  |   64   |   64    |  32  |    64     |   64   |  32   |  32   |   64   |
| Win64, gcc mingw64 LFF   |  8   |  16   |  32  |   64   |   64    |  32  |    64     |   64   |  64   |  32   |   64   |
| Win64, MSVC              |  8   |  16   |  32  |   64   |    -    |  32  |    64     |   64   |  32   |  32   |   64   |
| Linux64, gcc             |  8   |  16   |  32  |   64   |   64    |  64  |    64     |   64   |  64   |  32   |   64   |
| Linux64, gcc LFF         |  8   |  16   |  32  |   64   |   64    |  64  |    64     |   64   |  64   |  32   |   64   |

