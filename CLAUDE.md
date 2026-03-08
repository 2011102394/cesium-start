# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个基于 Vue 3 + TypeScript + Vite 的前端项目。

## 常用命令

```bash
# 启动开发服务器
pnpm dev

# 类型检查 + 构建生产版本
pnpm build

# 预览生产构建
pnpm preview
```

## 项目结构

```
src/
├── main.ts          # 应用入口，创建 Vue 实例
├── App.vue          # 根组件
├── style.css        # 全局样式
├── components/      # Vue 组件目录
└── assets/          # 静态资源
```

## 技术栈

- **Vue 3** - 使用 `<script setup>` 语法糖
- **TypeScript** - 启用严格模式 (`strict: true`)
- **Vite 7** - 构建工具
- **vue-tsc** - Vue TypeScript 类型检查

## TypeScript 配置

项目使用分离的 tsconfig 配置：
- `tsconfig.json` - 主配置，引用子配置
- `tsconfig.app.json` - 应用代码配置
- `tsconfig.node.json` - Vite/Node 配置文件

TypeScript 编译选项启用了 `noUnusedLocals`、`noUnusedParameters` 等严格检查。
