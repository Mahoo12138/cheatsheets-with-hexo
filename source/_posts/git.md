---
title: Git 常用操作手册
categories: Linux
version: 2.9.1
top: true
---

## Get Start

### user config

```bash
git config --global user.name "xxx"
git config --global user.email "xxx"
```

###### Set default editor

```bash
git config --global core.editor "vim"
```

### link remote repo

```bash
# 生成 ssh 密钥
ssh-keygen -t rsa -C "xxx@xxx.com"
```

```bash
# 检查连接
ssh -T git@xxx.com
```

## Commit

### amend commit date

```bash
git commit --amend --date="2024-01-26T09:51:07"
```

## Branch

### create new branch

```bash
git checkout -b feature/a
```
```bash
git checkout -b feature/b origin/master
```
```bash
git checkout --track origin/main
```

### detele local branch

```bash
git branch -d <branch-name>
```

### delete remote branch

```bash
git push origin --delete <branch-name>
```

### rename local branch

```bash
git branch -m oldName newName
```
### rename remote branch

```bash
# 重命名远程分支对应的本地分支
git branch -m oldName newName
```
```bash
# 删除远程分支
git push --delete origin oldName
```
```bash
# 上传新命名的本地分支
git push origin newName
```
```bash
# 把修改的本地分支与远程分支关联
git branch --set-upstream-to origin/newName
```

### unset upstream

```bash
git branch --unset-upstream
```


## Sync

### sync the upstream

```bash
# 添加一个远程分支作为上游仓库
git remote add upstream <upstream-url>
# 提交或暂存修改 
git commit / git stash
# 拉取上游分支改动
git fetch upstream
# 切换到主分支
git checkout master
# 将上游分支改动合并到本地主分支
git merge upstream/master
```

### replace remote repo

```bash
# 删除当前远程仓库关联
git remote rm origin
# 添加新的远程仓库
git remote add origin [repo-url]
# 验证更改
git remote -v 
```

## Tag

### create new tag

```bash
 git tag v1.0.0
```

### rename a tag

```bash
 # 基于旧标签创建新标签
 git tag <new-tag-name> <old-tag-name>
 # 删除旧的标签
 git tag -d <old-tag-name>
 # 同步到远程分支
 git push origin :refs/tags/<old-tag-name>
```

### sync tag to remote

```bash
 git push origin --tags
```

## Ignore

#### global ignore

```bash
git config --global core.excludesfile ~/.gitignore
```

