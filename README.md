# Taro WeApp Plugin

Claude Code 插件，提供 React to Taro 转换工具和微信小程序开发指南。

## 包含的 Skills

### 1. react-to-taro

将 React Web 应用转换为 Taro 4.x 小程序代码，包括：

- JSX 元素映射 (div→View, span→Text 等)
- 事件处理器转换 (onChange→onInput, e.target.value→e.detail.value)
- 路由/导航转换 (react-router-dom → Taro API)
- API 适配层 (axios→Taro.request, localStorage→Taro.setStorageSync)
- weapp-tailwindcss 配置指南

### 2. wechat-chat-tool

微信小程序聊天工具开发指南，包括：

- 聊天工具分包配置
- chatTools 配置
- 发送消息到群聊
- 动态消息
- 获取群成员信息

## 安装

### 方式 1：通过 Marketplace 安装

```shell
/plugin marketplace add dafang/taro-weapp-plugin
/plugin install taro-weapp-plugin@taro-weapp-plugin
```

### 方式 2：本地测试

```bash
claude --plugin-dir ./taro-weapp-plugin
```

## 使用

安装后，Skills 会自动在相关场景下激活：

- 当你需要将 React 代码转换为 Taro 时，使用 `/react-to-taro`
- 当你开发微信小程序聊天工具时，使用 `/wechat-chat-tool`

## License

MIT
