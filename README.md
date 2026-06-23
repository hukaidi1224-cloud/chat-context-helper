# 聊天语境助手 (Chat Context Helper)

一个纯前端的 AI 聊天辅助工具——为不同的聊天对象/场景保存语境卡片，让 AI 根据对象的性格、关系、说话风格生成高情商回复。

## 为什么需要这个？

现有的 AI 帮写工具只关注「怎么写」，忽略了「对谁写」。你跟 crush、老板、家人说话的方式完全不同——这个工具就是帮你记住这些差异，让 AI 的回复**像你，又懂对方**。

## 功能

- **语境卡片管理**：按人/场景创建卡片，记录对方性格、关系、说话风格、重要回忆、注意事项
- **多场景生成**：私信聊天（微信/QQ/短信）或邮件沟通
- **多种帮助模式**：生成回复、调整语气、给建议、分析对方想法
- **完全本地**：数据存储在浏览器 IndexedDB，不经过任何服务器
- **导出/导入**：备份语境卡片，可迁移到其他设备

## 使用方式

### 直接打开

下载 `index.html`，用浏览器直接打开即可。不需要任何构建工具或服务器。

### 配置 API

本工具使用 **OpenAI 兼容协议**，支持任意兼容的 API 服务：

- [DeepSeek](https://platform.deepseek.com/)
- [OpenAI](https://platform.openai.com/)
- [硅基流动](https://siliconflow.cn/)
- [智谱](https://open.bigmodel.cn/)
- 或任何自部署的兼容服务

在「设置」页面填入 API Base URL 和 Key 即可。

## 隐私与安全

- **所有数据存储在本地浏览器**（IndexedDB），没有任何网络上传或追踪
- **API Key 存于 IndexedDB**，仅在你主动调用 API 时使用
- **导出备份时**，API Key 默认不包含，需手动确认才会导出

### 安全提醒

1. 不要在公共/共享电脑上保存 API Key
2. 导出带 API Key 的备份文件后请妥善保管，不要上传到公开位置
3. 备份文件 `.gitignore` 已忽略，不会被意外提交

## 技术栈

- 纯 HTML/CSS/JavaScript（零依赖）
- IndexedDB 本地存储
- OpenAI 兼容 API 协议
- GitHub Pages 可直接部署

## License

MIT
