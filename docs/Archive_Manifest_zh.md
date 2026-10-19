# 材料及版本清单

归档整理日期：2026-10-19。研究论文版本：`1.0-publication-candidate`（2026-10-17）。

## 用户上传的五份输入文件

| 用户上传文件 | 预期归档名 | 字节数 | SHA-256 | GitHub 状态 |
| --- | --- | ---: | --- | --- |
| `Manuscript_zh(1).md` | `docs/Manuscript_zh.md` | 24218 | `b00b5965c9f16e1be702aa70ded9ba58c9357e6766d5671b4986569ecd619dd0` | 已上传文字原文 |
| `Audit_Report_zh(1).md` | `docs/Audit_Report_zh.md` | 5303 | `037b353e2678b08d8bbf8541d63c2ada467b1ff15ab058021383b6f748fd03c3` | 已上传文字原文 |
| `Empirical_Protocol_zh(1).md` | `docs/Empirical_Protocol_zh.md` | 4421 | `576f53132d0a988baecc058a1f3ef52fc7e80cff6bad695f3dfe13e6711c1c1c` | 已上传文字原文 |
| `TheLastOfUS_v1.0_Audit_and_Lab(1).xlsx` | `workbooks/TheLastOfUS_v1.0_Audit_and_Lab.xlsx` | 178896 | `5b19b6c1f1f55bac2696b09a046980b67509d9a5fc356c364e0dab7ad62f15dd` | **未上传二进制** |
| `Guangdong_payroll_AI_cost_2026_10(2).xlsx` | `workbooks/Guangdong_payroll_AI_cost_2026_10.xlsx` | 32738 | `869d352062b6e08039b22a575e6a806de9e532f85b9327a32f247e0a04217877` | **未上传二进制** |

上述 SHA-256 为上传文件的原始**字节级摘要**，不能用来校验 Markdown 经过 API 文本传输后是否保持原字节（例如编码或换行变动）；但可识别本轮输入版本。二进制工作簿依然是报告讨论对象，尚待可用的二进制上传通道补入。

## 工作簿内容索引

### 主工作簿（10 张工作表）

`00_Readme`、`01_Static`、`02_Liquidity`、`03_Mortgage`、`04_Audit`、`05_Sources`、`06_Regions`、`07_Experiments`、`08_Grid`、`09_Verification`。

### 广东微观账本（6 张工作表）

`结论与使用说明`、`城市与费率`、`反推实发5000`、`各险种最低基数`、`AI订阅对比`、`来源与限制`。

## 第三轮报告的归属和状态

第三轮 Argon 原文来自研究作者在本次对话中直接粘贴的消息，**不是**一个随附的独立 Markdown 原稿文件。归档者据其四部分叙述、C001–C006、模型命题、3.6/H4 草案与公式补丁编排为 [Argon_Third_Round_Audit_zh.md](Argon_Third_Round_Audit_zh.md)，保留原始论点、主要数字和公式，属于**结构性整理文本**，不是逐字无损抄录。特别是第 3.6 节已压缩重述；原始长文本应视为核对底本。

本轮不将 Argon 所称“独立复审”替代外部人工经济学审稿，不将建议补丁标记为完成，也不对 12 地的经验状态解锁。项目提及但未随本次附件提供的源代码和原始实验数据，不在本次归档范围内。