# 给 Claude 的说明

**当前仓库：VehDiag_gnl（General 通用版）**——功能和自用版（SEF）一致：故障码查询、报文数据分析（故障码识别、疑似异常、信号曲线、报文提取）、AI 助手。但仓库里只有代码，不含任何车型资料：DBC 和诊断问卷 Excel 都由使用者自己上传（只存在本机浏览器）。公开、不需要密码。

- 文件：`index.html`；`canlog.js`、`plot.js`、`ai.js` 与 SEF 的 `tools/web/` 同源，改了要同步；`dbc.js` 是 SEF `tools/dbc.py` 的 JS 版，`qn.js` 解析问卷，`uds.js` 是 SEF `tools/uds.json` 的副本；`诊断问卷模板.xlsx` 只放通用示例码。
- 不要把任何真实 DBC、问卷或报文放进这个仓库。

## 四个仓库的定位（同一个用户 gcy2016 的售后诊断工具系列）
| 仓库 | 含义 | 定位 | 网址 |
|---|---|---|---|
| VehDiag_pub | Public 公共版 | 给非专业人员自助查询故障码；没有报文解析和数据分析功能。打开即用，无密码 | https://gcy2016.github.io/VehDiag_pub/ |
| VehDiag_sef | Self 自用版 | 用户自己用；功能最多，加密内容也最多（网站数据用 6 位网站密码，原始 DBC / 问卷用长的原始文件密码） | https://gcy2016.github.io/VehDiag_sef/ |
| VehDiag_shr | Share 分享版 | 给有一定专业能力的人查看报文；只能看原始报文（另有 AI 助手），不带 DBC、不做解析。无密码 | https://gcy2016.github.io/VehDiag_shr/ |
| VehDiag_gnl | General 通用版 | 功能和自用版一致，但仓库里只有代码，DBC、诊断问卷都由使用者自己上传。无密码 | https://gcy2016.github.io/VehDiag_gnl/ |

## 通用规则（四个仓库相同）
- 仓库都是公开的：不要把任何密码写进文件、提交或 issue。
- 用户已同意四个仓库都可以直接推送到 `main`（推送前先在本地测试），不必走 PR。
- 需要在 GitHub 网页上操作时（改设置、Pages 等）交给 Muse（Meta 的 AI，用 gcy2016 账号操作）：在相关仓库开 issue，标题以“muse：”开头，写清楚逐步操作，请 muse 完成后回复并关闭；不要写 `@muse`（那是无关的陌生账号）。
- 用户偏好：功能够用就行，别做成大而全的 CANalyzer；配色以主题蓝为主；手机和电脑都要适配（手机不超出屏幕宽度、输入框字号 ≥16px，电脑布局合理）。能选报文的仓库（SEF、SHR、GNL）交互保持一致，改一个就同步改其他。
- 更完整的说明（报文分析流程、待办）见 VehDiag_sef 仓库的 CLAUDE.md。
