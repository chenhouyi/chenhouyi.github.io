---
title: 设置 npm 使用国内映像源的方法
date: 2016-11-06 16:33:20
tags:
---

在国内的网络环境下，npm 从默认源下载包的速度非常慢，甚至达到了让人抓狂的地步。这时，其实只要设置让 npm 使用国内的映像源就可以了，速度立刻飞了起来。

## Let's do it

**方法一：**

```
npm config set registry https://registry.npm.taobao.org
```

**方法二：**

```
npm --registry https://registry.npm.taobao.org
```

**方法三：**

编辑 `~/.npmrc` 文件

```
registry = https://registry.npm.taobao.org
```

## 可选的源

**映像源：**

- [cnpm](https://cnpmjs.org)：`https://r.cnpmjs.org` 
- [淘宝 NPM 映像](https://npm.taobao.org)：`https://registry.npm.taobao.org`

**默认源：**

- npm：`http://registry.npmjs.org`

## 如何查看 npm 当前使用的源？

```
npm config get registry
```

