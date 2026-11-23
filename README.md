# 你好，我是 Arthur

我的项目主要围绕 **Go 后端开发**，从电商交易中的订单与库存一致性，到 Agent Runtime 的工具调用与会话管理。我也关注服务如何部署、监控和验证。

## 代表项目

### [Agent Workflow V5 · 多 Agent 开发协作框架](https://github.com/WenqingSong/agent-workflow)

**已发布 v5.0.0。** 这个项目解决多轮 AI 辅助开发中的交接问题，让团队能核对审查记录对应的是哪次提交，以及当前代码是否满足交付条件。

- **协作流程**。用 Git 提交和仓库内的任务记录串起需求拆解、设计、实现、独立审查、人工审批和交付验证。
- **Go 校验器**。`workflow-check` 通过五个检查关卡核对 Git 状态与各阶段记录，帮助项目负责人判断是否可以推进或合并。
- **发布与接入**。提供可接入现有 Git 仓库的源码包、安装与升级工具，以及 Linux、macOS（Apple Silicon）和 Windows 的校验器二进制文件与 SHA-256 校验文件。

[查看 v5.0.0 发布与下载](https://github.com/WenqingSong/agent-workflow/releases/tag/v5.0.0) · [安装与升级](https://github.com/WenqingSong/agent-workflow#安装与升级)

### [SurgeCart · 电商交易与秒杀后端](https://github.com/WenqingSong/my-shop)

基于 **GoFrame、MySQL、Redis 和 Kafka**。普通订单通过 MySQL 事务、条件更新和幂等键处理扣库存与重复请求。秒杀用 Redis Lua 做准入，支持通过 MySQL 请求表或 Kafka 异步落单，并记录失败后的重试与补偿。项目也提供 Docker Compose、本地 kind 部署和 Prometheus / Grafana 监控。

[订单设计](https://github.com/WenqingSong/my-shop/blob/main/docs/design/order.md) · [秒杀设计](https://github.com/WenqingSong/my-shop/blob/main/docs/design/flash-sale.md)

### [mini-agent-go · Go Agent Runtime](https://github.com/WenqingSong/mini-agent-go)

用 Go 实现多轮 Tool Calling，覆盖工具注册、参数校验、执行和结果回填。运行时管理会话隔离、调用预算和超时取消。项目带有 React 对话界面，前后端可打包为一个镜像。

## 个人作品集

[my-station](https://github.com/WenqingSong/my-station) 基于 React、TypeScript、Vite 和 GSAP，包含项目展示与 Agent Workflow 技术文档。
