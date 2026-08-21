# Gravity‑Booster

Gravity‑Booster 是灵狐雪维护的 Pi‑hole / hosts 广告拦截订阅（blocklist），针对 Android 应用与常见网站的广告与跟踪域名做了融合与清洗，便于在 Pi‑hole、AdGuard、路由器 hosts 等环境中订阅并使用。

- 订阅（Raw）：https://raw.githubusercontent.com/lhuxue/Gravity-Booster/main/blocklist.txt
- 当前收录：4949 条域名（清洗日期：2026-08-21）
- 参考 / 合并来源示例：SM‑Ad‑FuckU‑hosts 等多个公开 blocklist/hosts 项目
- 许可证：MIT（见 LICENSE）
- 作者：灵狐雪（lhuxue）

## 快速使用
1. 在 Pi‑hole 管理界面 -> Group Management -> Adlists 中添加订阅 URL（上述 Raw 链接），或将 blocklist.txt 的内容作为 hosts/blacklist 导入你的广告过滤器/路由器。
2. 更新并生效后，系统会屏蔽列表中的广告与跟踪域名。

## 说明与注意事项
- 该订阅以屏蔽效果为优先，可能存在误杀（某些图片、更新、功能或第三方服务会被一并阻断）。
- 使用前建议备份当前 hosts / Adlist 配置，并在出现问题时通过白名单或移除单条域名恢复功能。
- 如果你依赖某个被屏蔽的服务（例如地图图标、应用更新、第三方登录等），请在 Pi‑hole 或你的过滤器中把对应域名加入白名单。

## 贡献与反馈
欢迎提交 Issue 或 Pull Request 来改进规则、报告误杀或贡献新的来源。请在提交时提供可复现的抓包示例或受影响的具体域名/场景，以便准确评估。

## 致谢
感谢 SM‑Ad‑FuckU‑hosts 等原始规则作者与社区贡献者，列表融合与清洗基于多个公开来源。

## 许可证
本仓库采用 MIT 许可证，详见 LICENSE 文件。
