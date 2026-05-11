# ai-mental-health-assistant
基于 Vue 3 + JavaScript + Element Plus 开发的心理健康管理平台。通过 AI 实现流式对话咨询，并利用 ECharts 将情绪波动可视化。项目包含完整的前台用户交互与后台数据管理。

## 🌐 访问与演示

* **在线演示**: [点击进入项目](https://yangcancan0211.github.io/ai-mental-health-assistant/)
* **仓库地址**: [GitHub Repository](https://github.com/Yangcancan0211/ai-mental-health-assistant)

### 🔐 演示账户

| 角色 | 账号 | 密码 | 权限范围 |
| --- | --- | --- | --- |
| **后台管理员** | `admin` | `123456` | 全局数据大盘、用户管理、知识库运维 |
| **前台用户** | `122` | `111111` | AI 咨询、个人情绪趋势、日历记录 |
| **游客** | 支持自主注册 | - | 基础功能体验 |

---

## ✨ 项目双端核心特色

### 1. 🌈 前台用户端：沉浸式治愈交互 (C-End)

* **🤖 AI 深度对话**：基于自定义渲染引擎，支持流式 Markdown 回复，提供丝滑、专业的咨询体验。
* **📈 情绪日志**：日历式记录点滴心情，AI 根据历史对话自动生成每日小结。
* **📅 智能情绪日记**：支持基于日历视图的心情记录，AI 自动根据对话生成总结，辅助自我复盘。

### 2. 📊 后台管理端：多维数据赋能 (B-End)

* **🧭 情绪趋势分析**：通过折线图实时监控全平台用户情绪均值波动。
* **📊 咨询会话统计**：量化分析咨询时长、活跃用户数及会话分布，辅助决策。
* **📑 知识库运营**：支持心理科普文章的 CRUD 管理，动态触达前端用户。
* **🔐 权限架构**：完备的动态路由拦截，确保管理员与普通用户的数据隔离。

---

## 🛠️ 技术栈清单

* **核心框架**: Vue 3.4+ (Composition API)
* **UI 组件库**: Element Plus (深度定制治愈系浅色主题)
* **可视化引擎**: **ECharts ** (封装响应式图表组件)
* **状态管理**: Pinia (处理用户状态持久化与 token 管理)
* **路由管理**: Vue Router (Hash 模式，完美兼容静态托管)
* **网络请求**: Axios (按模块封装拦截器，支持前后端分离接口)

---

## 📂 项目结构

```text
├── public/              # 静态资源 (如 favicon.svg)
├── src/                 # 源代码目录
│   ├── api/             # 接口请求封装 (JS 封装)
│   ├── assets/          # 本地静态资源 (图片、全局样式)
│   ├── components/      # 公共 UI 组件
│   │   ├── charts/      # 基于 ECharts 封装的图表组件
│   │   └── ...
│   ├── config/          # 全局配置 (如环境变量)
│   ├── router/          # 路由配置 (index.js)
│   ├── stores/          # Pinia 状态管理 (如 admin.js)
│   ├── utils/           # 工具函数封装
│   ├── views/           # 业务页面 (前台与后台页面)
│   ├── App.vue          # 根组件
│   ├── main.js          # 入口文件
│   └── style.css        # 全局样式
├── .gitignore           # Git 忽略配置
├── .nojekyll            # 绕过 GitHub Pages 检查 (关键)
├── index.html           # 页面入口
├── jsconfig.json        # JS 路径提示配置
├── package.json         # 项目依赖与脚本
└── vite.config.js       # Vite 配置文件

```

---

## 🚀 开发者快速启动

1. **克隆仓库**
```bash
git clone https://github.com/Yangcancan0211/ai-mental-health-assistant.git

```


2. **安装依赖**
```bash
npm install

```


3. **本地开发**
```bash
npm run dev

```


4. **编译生产环境**
```bash
npm run build
