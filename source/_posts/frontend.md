---
title: 前端工具常用命令
categories: Programming
version: 1.0
top: true
---

#### Yarn

```bash
# 查询源
yarn config get registry
# 删除
yarn config delete registry
```
```bash
# 更换国内源
yarn config set registry https://registry.npmmirror.com
# 恢复官方源
yarn config set registry https://registry.yarnpkg.com
```
```bash
# 添加代理
yarn config set proxy http://127.0.0.1:7890
yarn config set https-proxy http://127.0.0.1:7890
# 删除代理
yarn config delete proxy
yarn config delete https-proxy
```

#### Npm

```bash
# 查询源
npm config get registry
# 删除源
npm config delete registry
```
```bash
# 更换国内源
npm config set registry https://registry.npmmirror.com
# 恢复官方源
npm config set registry https://registry.npmjs.org
```
```bash
# 添加代理
npm config set proxy http://127.0.0.1:7890
npm config set https-proxy http://127.0.0.1:7890
# 删除代理
npm config delete proxy
npm config delete https-proxy
```
注意 npm 更换国内镜像源之后，将无法再使用 `npm search` 命令，需要恢复为官方源才可以使用，如果恢复官方源后还不可使用，运行删除注册表命令后重试即可。

#### Pnpm

```bash
# 查看源
pnpm get registry
pnpm config get registry

# 临时修改
pnpm --registry https://registry.npmmirror.com install any-touch

# 永久修改
pnpm config set registry https://registry.npmmirror.com

# 还原
pnpm config set registry https://registry.npmjs.org

pnpm config set global-bin-dir "D:\Cache\.pnpm-store"
pnpm config set cache-dir "D:\Cache\.pnpm-store\cache"
```
### Yarn Workspace - v1

```bash
# 在指定的 workspace 下执行命令
yarn workspace <workspace_name> <command>
```

```bash
# 遍历所有 workspace 执行 command 命令
yarn workspaces run <command>
```

### Yarn Workspace - v2
```bash
# 安装单个工作区及其依赖项
yarn workspaces focus
```

```bash
# 在 workspace-root 下执行，列出所有可用的工作区
yarn workspaces list
```