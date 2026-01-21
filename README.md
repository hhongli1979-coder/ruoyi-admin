# 若依AI管理系统 (RuoYi AI Admin)

> [English Documentation](./README_EN.md) | 中文文档

基于 Vben Admin 框架构建的现代化后台管理系统，集成了完整的权限管理、系统监控等企业级功能模块。

## ✨ 项目特性

- 🎯 **现代化架构**：基于 Vue 3 + TypeScript + Vite 构建
- 🛠️ **丰富组件**：集成 Ant Design Vue 组件库
- 🔐 **权限管理**：完整的 RBAC 权限控制体系
- 📊 **系统监控**：实时监控系统运行状态
- 📱 **响应式设计**：完美适配各种设备屏幕

## 🚀 技术栈

### 前端技术
- **Vue 3** - 渐进式 JavaScript 框架
- **TypeScript** - JavaScript 的超集
- **Vite** - 下一代前端构建工具
- **Ant Design Vue** - 企业级 UI 组件库
- **Pinia** - Vue 状态管理
- **Vue Router** - 官方路由管理器

### 开发工具
- **pnpm** - 快速、节省磁盘空间的包管理器
- **Turbo** - 高性能构建系统
- **ESLint** - 代码质量检查
- **Prettier** - 代码格式化
- **Husky** - Git hooks 工具

## 📋 环境要求

- **Node.js** >= 20.10.0
- **pnpm** >= 9.12.0

## 🛠️ 快速开始

### 1. 克隆项目
```bash
git clone https://gitee.com/ageerle/ruoyi-admin
cd ruoyi-admin
```

### 2. 安装依赖
```bash
pnpm install
```

### 3. 启动开发服务器
```bash
pnpm run dev:antd
```

### 4. 构建生产版本
```bash
pnpm run build:antd
```

## 🧩 后端源码合并与 Runpad 部署

### 后端源码合并
1. 将后端仓库合并到当前项目根目录的 `backend/`（示例路径，可按团队约定调整）。
2. 保持前后端依赖独立：前端继续使用 `pnpm`，后端保持原有构建/运行方式。
3. 按后端地址更新前端环境变量（例如 `.env*` 中的 `VITE_API_URL`）。

### Runpad 部署（合并后）
1. 确保 Runpad 源码随后台合并到 `backend/runpad`（或团队约定路径）。
2. 按 Runpad 目录中的 README/部署脚本配置环境变量（数据库、缓存、密钥等）。
3. 在服务器上执行 Runpad 的启动命令或容器部署命令，确认端口与后台主服务不冲突（按 Runpad README 中的端口配置检查）。
4. 在后台配置中填写 Runpad 服务地址（参考后端配置文件或环境变量的服务地址字段），确保联调正常。

## 📝 注意事项

1. **Node.js 版本**：请确保使用 Node.js 20.10.0 或更高版本
2. **包管理器**：项目使用 pnpm，请勿使用 npm 或 yarn
3. **开发环境**：推荐使用 VS Code 并安装相关插件
4. **浏览器支持**：支持现代浏览器，不支持 IE

## 📚 项目结构

```
ruoyi-admin/
├── apps/                    # 应用目录
│   ├── web-antd/           # Ant Design Vue 版本
├── packages/               # 共享包
│   ├── @core/             # 核心包
│   ├── constants/         # 常量定义
│   ├── effects/           # 副作用处理
│   ├── icons/             # 图标库
│   ├── locales/           # 国际化
│   ├── preferences/       # 偏好设置
│   ├── stores/            # 状态管理
│   ├── styles/            # 样式文件
│   ├── types/             # 类型定义
│   └── utils/             # 工具函数
├── internal/              # 内部工具
└── scripts/               # 构建脚本
```

---

**若依AI管理系统 - 让企业级后台管理更简单、更高效！**
