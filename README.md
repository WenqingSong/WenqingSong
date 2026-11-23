# 你好，我是 Arthur

我的项目主要围绕 **Go 后端开发**，从电商交易中的订单与库存一致性，到 Agent Runtime 的工具调用与会话管理。我也关注服务如何部署、监控和验证。

## 代表项目

### [SurgeCart · 电商交易与秒杀后端](https://github.com/WenqingSong/my-shop)

基于 **GoFrame、MySQL、Redis 和 Kafka**。普通订单通过 MySQL 事务、条件更新和幂等键处理扣库存与重复请求。秒杀用 Redis Lua 做准入，支持通过 MySQL 请求表或 Kafka 异步落单，并记录失败后的重试与补偿。项目也提供 Docker Compose、本地 kind 部署和 Prometheus / Grafana 监控。

[订单设计](https://github.com/WenqingSong/my-shop/blob/main/docs/design/order.md) · [秒杀设计](https://github.com/WenqingSong/my-shop/blob/main/docs/design/flash-sale.md)

### [mini-agent-go · Go Agent Runtime](https://github.com/WenqingSong/mini-agent-go)

用 Go 实现多轮 Tool Calling，覆盖工具注册、参数校验、执行和结果回填。运行时管理会话隔离、调用预算和超时取消。项目带有 React 对话界面，前后端可打包为一个镜像。

### [Agent Workflow · AI 辅助开发协作](https://github.com/WenqingSong/agent-workflow)

用 Git 提交和仓库内的任务文件串起设计、实现、审查和交付。Go 校验器检查当前提交与审查记录，关键步骤由项目负责人决定是否继续。

## 个人作品集

[my-station](https://github.com/WenqingSong/my-station) 基于 React、TypeScript、Vite 和 GSAP，包含项目展示与 Agent Workflow 技术文档。
