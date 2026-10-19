# Argon 第三轮审计追踪清单（2026-10-19 整理）

本表是第三轮报告的**问题索引**，不是已经通过修复验收的清单。主报告：[Argon 第三轮复审](Argon_Third_Round_Audit_zh.md)。

| ID | 优先级 | 定位 | Argon 所述现象 | 提议处置 | 本次发布状态 |
| --- | --- | --- | --- | --- | --- |
| C001 | P1 | 主工作簿 `08_Grid` | 432 组网格快照漏列单位成本改善率 η | 补字段并重导快照 | REPORTED_BY_ARGON / NOT_APPLIED |
| C002 | P1 | 主工作簿 `07_Experiments` | `buy_fixed_dual` 与 `buy_defer_dual` 结果重合、购前检查非绑定 | 新增购前/购房同期冲击绑定测试，保留旧对照 | REPORTED_BY_ARGON / NOT_APPLIED |
| C003 | P1 | 主工作簿 `02_Liquidity` | 负余额仍按 1% 储蓄收益率递推 | 区分未融资缺口与实际借贷，分段利率或停止复利 | REPORTED_BY_ARGON / NOT_APPLIED |
| C004 | P2 | 论文 `3.3` | 价格弹性下福利与可偿债现金可能不同 | 补 `B[1-(1-λκη)^(1-ε)]` 现金释放公式 | PROPOSED / NOT_APPLIED |
| C005 | P2 | 广东账本 `反推实发5000` | 九轮固定点迭代存在小额尾差 | 核验并替换为适用分段的闭式解 | PROPOSED / NOT_APPLIED |
| C006 | P2 | 主工作簿 `03_Mortgage` | 月度实际月供与年度流动性尺度不同 | 提供逐年汇总列和现金流时点说明 | PROPOSED / NOT_APPLIED |

## 建议增补与配套追踪

| 编号 | 建议位置 | 内容 | 状态 |
| --- | --- | --- | --- |
| P-3.6 | `Manuscript_zh.md` 第 3.5 节之后 | 制度楔子、缴费下限、专款流动性 | DRAFT_ONLY |
| P-H4 | `Empirical_Protocol_zh.md` 第 2 节 | 制度楔子与企业调整边际待检验假说 | DRAFT_ONLY |
| P-WB | 广东账本 `N` 列 | 免税段分段线性闭式反推 | DRAFT_ONLY |
| P-CHN | 中国/广东制度参数适配器 | 参数核验 + 微观样本 + 外部对照 | BLOCKED |

说明：`P1/P2` 为 Argon 报告的优先级。`REPORTED_BY_ARGON` 表示该判断来自第三轮原报告，不表示本次归档者已对所有轨迹重新验算。项目既有的 v1.0 `04_Audit` 表未改写；编号在此独立保留，待后续合并。