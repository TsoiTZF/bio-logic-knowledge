# CHANGELOG

## 2026-09-12 (v1.1)

与 bio-logic-debugger 内置库对齐。

- traits：18 → 40；亩产单位改为 kg/亩；SES 1–9 级标明越大越差（`higher_is_better: false`）
- correlations：13 → 30；补 evidence
- constraints：3 → 9；补 evidence 与完整 condition_expr
- anti_patterns：5 → 7；补 evidence / failed_approaches

应用侧改为手动同步，写入用户目录，不再启动时自动覆盖。

## 2026-04-28 (v1.0)

初始版本，基于 rice_knowledge.py 内置知识库导出。

### traits.json
- 18 个性状：产量、品质、株型、抗病、生育期、抗逆
- 覆盖水稻主要育种目标维度

### correlations.json
- 13 条性状关联
- 包含正相关、负相关、权衡关系、曲线关系

### constraints.json
- 3 条生物学约束规则（FATAL 级）

### anti_patterns.json
- 5 个反模式
- 覆盖高产低质陷阱、极端粒型、过度矮化、早熟必低产、全面抗病性价比陷阱