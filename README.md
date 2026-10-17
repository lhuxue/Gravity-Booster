# Gravity‑Booster

Gravity‑Booster 是灵狐雪（lhuxue）维护的 Pi‑hole / hosts 广告拦截订阅（blocklist），针对 Android 应用与常见网站的广告与跟踪域名做了融合与清洗，便于在 Pi‑hole、AdGuard、路由器 hosts 等环境中订阅并使用。

- [订阅](https://raw.githubusercontent.com/lhuxue/Gravity-Booster/main/blocklist.txt)（Raw）
- 参考 / 合并来源：详见致谢部分，主要来自公开 blocklist/hosts 项目
- 许可证：MIT（见 LICENSE），与上游保持兼容，上游使用各自的许可证

## 快速使用
1. 在 Pi‑hole 管理界面 -> Group Management -> Adlists 中添加订阅 URL（上述 Raw 链接），或将 blocklist.txt 的内容作为 hosts/blacklist 导入你的广告过滤器/路由器。
2. 更新并生效后，系统会屏蔽列表中的广告与跟踪域名。

## 说明与注意事项
- 该订阅以屏蔽效果为优先，可能存在误杀（某些图片、更新、功能或第三方服务会被一并阻断）。
- 使用前建议备份当前 hosts / Adlist 配置，并在出现问题时通过白名单或移除单条域名恢复功能。
- 如果你依赖某个被屏蔽的服务（例如地图图标、应用更新、第三方登录等），请在 Pi‑hole 或你的过滤器中把对应域名加入白名单。

## 致谢
感谢这些原始规则作者与社区贡献者，列表融合与清洗基于公开来源。

|名称|主页|订阅链接|
|:---|:---|:---|
|SM‑Ad‑FuckU‑hosts|[主页](https://github.com/2Gardon/SM-Ad-FuckU-hosts/blob/master/SMAdHosts)|[订阅](https://raw.githubusercontent.com/2Gardon/SM-Ad-FuckU-hosts/refs/heads/master/SMAdHosts)|
