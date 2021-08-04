# pomo lite
一款简单的基于 `electron`、`react`和`vite`的番茄钟

### start

```shell
$ yarn # or npm i

# 使用 esbuild 来编译主进程 Typescript，速度更佳
yarn run dev

# 使用 tsc 来编译主进程 Typescript
yarn run dev:tsc
```

也可以分开使用 `dev:main`, `dev:main:tsc`, `dev:renderer` 来分开调试主进程和渲染进程。

编译/打包

```shell
# 仅构建主进程和渲染进程的目标代码和资源，不打包（exe, dmg 等）
yarn run build

# 在 build 的基础上运行/预览运行效果 (production 模式)，用来本地验证
yarn run preview

# 构建并打包为可运行的程序或安装程序
yarn run pack:win
yarn run pack:mac
yarn run pack:linux

# 为所有平台打包
yarn run pack # 排除 mac 平台，适用于 linux & win
yarn run pack:all
```

清理构建目录

```shell
yarn run clean
```

### todo
- [x] 实现休息
- [x] 实现四个番茄钟后一个长休息
- [x] 番茄钟可暂停
- [ ] 可存储数据
- [ ] 展示历史番茄钟
- [ ] UI美化
- [ ] 暗黑模式