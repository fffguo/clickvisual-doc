# 变更日志

## ClickVisual 版本 2022-09-30 v0.4.2

[https://github.com/clickvisual/clickvisual/releases/tag/v0.4.2](https://github.com/clickvisual/clickvisual/releases/tag/v0.4.2)

### 新功能
- 增加对链路日志库数据分析功能
- 用户管理模块，基础 CURD 和用户密码重置功能

### 改进
- clickhouse-go 升级为 v2.3.0，并支持 http 和 https 协议 [@laojianzi](https://github.com/laojianzi)
- 优化已接入日志时间字段筛选逻辑，使用 like 方式进行过滤 [@shushenghong](https://github.com/shushenghong)
- 链路日志库增加更多数据展示
- 一般日志库与链路日志库跳转交互优化
- 从分析日志内容格式来确认日志库类型，调整为通过具体的用户配置来进行确认
- 告警列表支持 id 过滤，避免同名产生的误导
- 删除对集群中非必要数据进行的 watch 逻辑
- 针对大量数据的缓慢日志渲染进行了优化

### 修复
- 链路日志库分析落地数据库创建失败问题
- 对不同时间区间使用不同的时间精度来显示时间点
