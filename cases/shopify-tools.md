# Shopify 工具平台

角色：平台设计与全栈开发

## 背景

主题开发、Shopify 后台操作、权限分配和发布记录分散，技术与非技术同事难以安全复用统一工作流。

## 关键工作

- 将 Shopify Admin MCP、Theme Tools、管理门户和共享协议整合为 Monorepo
- 实现企业身份系统 OAuth、基于角色与店铺的权限控制，并让一个应用承载企业用户各自的 Admin API 权限
- 建设 Windows 桌面应用与 CLI，覆盖主题拉取、预览、编辑、推送、回滚和 Skills 部署
- 把 版本仓库 版本记录、签名制品、哈希校验、测试晋级和生产发布纳入统一流程

## 结果

- 形成面向企业内部团队的 Shopify 管理与主题工具平台，统一身份、权限、桌面端、CLI 和发布链路。
- 将敏感凭据限制在服务端或进程内存，并通过短期令牌、审计和签名制品降低误操作与供应链风险。

技术：TypeScript、React、Tauri、Rust、Node.js、MCP、OAuth 2.0、RBAC、Shopify API、CI/CD
