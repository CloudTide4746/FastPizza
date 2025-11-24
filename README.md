# Fast React Pizza Co.

一个使用 React、Redux Toolkit 和 React Router DOM 构建的现代化、响应式的披萨订购应用程序。该应用程序允许用户浏览披萨菜单、将商品添加到购物车并下单配送。

## 🍕 功能特性

- **浏览披萨菜单**：查看各种美味披萨的图片、描述和价格
- **购物车**：添加/删除商品，调整数量，查看购物车总计
- **下单**：填写客户信息和配送地址的完整订单表单
- **订单跟踪**：查看订单状态和预计送达时间
- **优先订单**：可选择升级订单以获得更快的配送服务
- **地理位置**：使用浏览器地理位置自动检测地址
- **响应式设计**：使用 Tailwind CSS 构建的移动友好界面

## 🛠️ 使用的技术

- **React** - 用于构建用户界面的前端库
- **Redux Toolkit** - 状态管理解决方案
- **React Router DOM** - React 应用程序的声明式路由
- **Tailwind CSS** - 实用优先的 CSS 框架
- **Vite** - 快速的构建工具和开发服务器
- **ESLint & Prettier** - 代码检查和格式化工具

## 📁 项目结构

```
src/
├── features/
│   ├── cart/       # 购物车功能
│   ├── menu/       # 披萨菜单展示
│   ├── order/      # 订单下单和跟踪
│   └── user/       # 用户信息和地理位置
├── services/       # API集成
├── ui/             # 可复用的UI组件
├── utils/          # 辅助函数
├── App.jsx         # 主应用程序组件
├── main.jsx        # 应用程序入口点
└── store.js        # Redux store配置
```

## 🚀 开始使用

### 先决条件

- Node.js (v14 或更高版本)
- npm 或 yarn

### 安装

1. 克隆仓库：

   ```bash
   git clone https://github.com/CloudTide4746/FastPizza
   ```

2. 进入项目目录：

   ```bash
   cd FastPizza
   ```

3. 安装依赖：
   ```bash
   npm install
   ```

### 开发

启动开发服务器：

```bash
npm run dev
```

应用程序将在 `http://localhost:5173` (或下一个可用端口) 上访问。

### 生产构建

创建生产构建：

```bash
npm run build
```

预览生产构建：

```bash
npm run preview
```

## 🎯 核心功能

### 菜单浏览

- 用户可以查看所有可用的披萨及其详细信息
- 菜单项显示图片、配料和价格
- 售罄商品有明确标记

### 购物车

- 将披萨添加到购物车并选择数量
- 调整商品数量或删除商品
- 实时计算购物车总额
- 清空购物车功能

### 订单流程

1. **客户信息**：输入姓名和电话号码
2. **配送地址**：手动输入或自动地理位置检测
3. **订单优先级**：可选的优先服务以获得更快配送
4. **订单确认**：查看并提交订单

### 订单管理

- 查看带有唯一订单 ID 的订单详情
- 跟踪订单状态（准备中、制作中、已完成、已取货）
- 查看预计送达时间
- 将普通订单升级为优先订单

## 🔧 Redux 状态管理

应用程序使用 Redux Toolkit 进行状态管理，包含以下切片：

- **Cart Slice**：管理购物车商品和计算
- **User Slice**：处理用户信息和地理位置数据
- **Menu Slice**：存储从 API 获取的菜单数据

## 🌐 路由

应用程序实现了客户端路由，包含以下路径：

- `/` - 首页
- `/menu` - 披萨菜单
- `/cart` - 购物车
- `/order/new` - 创建新订单
- `/order/:orderId` - 订单详情

## 📱 响应式设计

使用 Tailwind CSS 构建，确保应用程序在以下设备上无缝运行：

- 台式电脑
- 平板电脑
- 移动设备

## 🤝 贡献

1. Fork 仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📄 许可证

该项目基于 MIT 许可证 - 详情请见 LICENSE 文件。

## 🙏 致谢

- 遵循现代 React 最佳实践构建
- 使用 React Router 实现无缝导航
- 实现 Redux Toolkit 进行高效的状态管理
