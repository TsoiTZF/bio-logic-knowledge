# Bio-Logic Debugger 社区知识库

供 [bio-logic-debugger](https://github.com/TsoiTZF/bio-logic-debugger) 手动同步使用。

应用**不会**在启动时自动覆盖本地知识。用户点「检查更新」后，文件写入 `~/.bio-logic-debugger/community/`，内置 JSON 不会被改掉。

## 文件

| 文件 | 内容 |
| --- | --- |
| `traits.json` | 性状 |
| `correlations.json` | 性状关联 |
| `constraints.json` | 生理约束（`condition_expr`） |
| `anti_patterns.json` | 历史反模式 |

最低字段：性状要有 `id`/`name`；关联要有 `trait_a`/`trait_b`/`corr_type`/`strength`；约束要有 `id`/`name`/`severity`；反模式要有 `id`/`name`/`trigger_traits`。校验失败的文件不会写入用户目录。

当前规模：性状 40、关联 30、约束 9、反模式 7。与调试器内置库对齐。

水稻示例库。亩产正式 id 为 `rice_yield_per_mu`，单位 **kg/亩**；`rice_yield_per_ha` 仍可作为别名。相关系数多为示意量级。无 URL 的证据不标 CONFIRMED。抗病/抗逆 `级` 为 IRRI SES：1 优/抗，9 劣/感。垩白度越低越好。
