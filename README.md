# 简易后端管理系统 (Admin Dashboard)

一个基于 Next.js + TypeScript + Ant Design 的现代化后端管理系统。

## 功能特性

### 🔐 用户认证
- 用户登录/登出
- 基于角色的权限控制
- 路由保护

### 👥 用户管理
- 用户的增、删、改、查 (CRUD)
- 用户信息包括：用户名、邮箱、角色、状态
- 支持分页、搜索、排序
- 表单验证

### 📊 仪表盘
- 数据统计展示
- 用户分布图表
- 最近用户列表

### 🎨 UI/UX
- 使用 Ant Design 组件库
- 响应式设计
- 现代化界面

## 技术栈

- **前端框架**: Next.js 14 (App Router)
- **语言**: TypeScript
- **UI 组件库**: Ant Design
- **状态管理**: Zustand
- **样式**: Tailwind CSS
- **表单处理**: React Hook Form

## 快速开始

### 安装依赖

```bash
npm install
```

### 开发环境运行

```bash
npm run dev
```

### 构建生产版本

```bash
npm run build
```

### 启动生产版本

```bash
npm start
```

## 测试账号

- **管理员**: admin / 123456
- **普通用户**: user / 123456

## 项目结构

```
src/
├── app/                 # Next.js App Router 页面
│   ├── dashboard/       # 仪表盘页面
│   ├── login/          # 登录页面
│   ├── users/          # 用户管理页面
│   ├── globals.css     # 全局样式
│   ├── layout.tsx      # 根布局
│   └── page.tsx        # 首页
├── components/         # React 组件
│   ├── Dashboard.tsx   # 仪表盘组件
│   ├── Layout.tsx      # 布局组件
│   ├── LoginForm.tsx   # 登录表单
│   ├── UserForm.tsx    # 用户表单
│   └── UserManagement.tsx # 用户管理
├── lib/               # 工具函数
│   └── utils.ts       # 通用工具
├── store/             # 状态管理
│   ├── auth.ts        # 认证状态
│   └── users.ts       # 用户状态
└── types/             # TypeScript 类型定义
    └── index.ts       # 类型定义
```

## 主要功能说明

### 1. 用户认证
- 使用 Zustand 进行状态管理
- 支持本地存储持久化
- 路由级别的权限控制

### 2. 用户管理
- 完整的 CRUD 操作
- 实时搜索和过滤
- 分页和排序
- 表单验证

### 3. 权限控制
- 基于角色的访问控制
- 不同角色可访问不同页面
- 前端路由保护

### 4. 数据管理
- Mock 数据模拟真实 API
- 状态管理优化
- 数据持久化

## 开发说明

### 添加新功能
1. 在 `src/types/` 中定义类型
2. 在 `src/store/` 中添加状态管理
3. 在 `src/components/` 中创建组件
4. 在 `src/app/` 中添加页面路由

### 样式定制
- 使用 Tailwind CSS 进行样式定制
- Ant Design 组件样式可通过 CSS 变量覆盖

### 状态管理
- 使用 Zustand 进行轻量级状态管理
- 支持持久化存储
- 类型安全的状态更新

## 部署

### Vercel 部署
1. 将代码推送到 GitHub
2. 在 Vercel 中导入项目
3. 自动部署

### 其他平台
1. 运行 `npm run build`
2. 将 `.next` 文件夹部署到服务器
3. 配置环境变量

## 贡献

欢迎提交 Issue 和 Pull Request！

## 许可证

MIT License 