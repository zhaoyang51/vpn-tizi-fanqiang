# 全平台科学上网客户端配置与 AI 防风控分流指南

本指南适用于 Clash Verge Rev、Mihomo Party、Shadowrocket（小火箭）等主流跨平台客户端，帮助解决日常连接中的漏网直连、AI 工具地区受限及节点切换问题。

---

## 1. Windows / macOS：开启 TUN 模式（强烈推荐）

使用 Google Antigravity、Claude Code、Cursor、Git、Docker 或桌面端软件时，仅开启「系统代理」常常无效，必须开启 **TUN 模式（虚拟网卡接管）**：

1. 打开客户端（如官方客户端或 Clash Verge Rev / Mihomo Party）。
2. 进入 **设置 / 常规配置**，首次开启需点击 **安装服务模式（Service Mode）** 并授权管理员权限。
3. 打开 **TUN 模式** 开关，确保规则模式设为 **Rule（规则分流）**。
4. 如遇 AI 工具依然提示区域受限，可在分流规则中强制将 `google.com`、`anthropic.com`、`openai.com`、`cursor.sh` 指定走 **纯净美国（US）原生节点**。

---

## 2. iOS：Shadowrocket（小火箭）建议配置

- **全局路由**：建议选 **配置（Config）**，兼顾国内网站直连与海外代理加速。
- **按需测速**：定期点击「连通性测试」，优先选择延迟低且支持流媒体/AI 的美国或新加坡原生节点。

---

## 3. 节点地区选择建议

| 目标应用 | 推荐节点地区 | 注意事项 |
| :--- | :--- | :--- |
| **Google Antigravity / Gemini / Codex** | **美国（US）** | 尽量固定同一条干净节点，避免频繁跨国切换触发安全校验 |
| **Claude / Cursor / OpenAI ChatGPT** | **美国 / 新加坡 / 日本** | 避免使用香港（HK）和俄罗斯节点 |
| **TikTok 运营 / 跨境电商** | **目标运营国家原生节点** | 配合独立浏览器环境与原生住宅 IP 使用 |
| **X (Twitter) / YouTube 高清视频** | **香港 / 日本 / 台湾 / 新加坡** | 延迟最低、带宽最充裕，适合大流量观影 |
