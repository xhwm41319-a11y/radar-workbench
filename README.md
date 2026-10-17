# RADAR Digital — Research Evidence Workbench

把已有 Solana 研究资料整理成包含来源声明、覆盖范围和未知项的研究卡。面向研究者、社区管理员和教程作者。

Turn existing Solana research material into reviewable cards with source declarations, coverage and unknowns. For researchers, community moderators and tutorial authors.

**本地试用候选 / Local trial candidate:** 主包 0.3.4；内含中英文浏览器页面沿用 0.3.3。0.3.4 的改动在 Python 区块导入路径，不能据此称网页新增功能。

## Start / 从这里开始

1. 在本仓库的 [Releases](https://github.com/xhwm41319-a11y/radar-workbench/releases) 列表查找 `RADAR-链上研究证据工作台-0.3.4-候选.zip`。只有附件实际可见、可下载，才算入口可用；没有附件时请勿把仓库源码 ZIP 当成产品包。
2. 解压到一个新文件夹，按 [首次使用说明 / First run](FIRST-RUN.md) 完成一次虚构样例和导出。
3. 用 [SHA256SUMS.txt](SHA256SUMS.txt) 核对下载文件；具体字节数见 [release-assets.json](release-assets.json)。这只证明文件一致，不证明链上来源或安全性。

Find the named product ZIP in Releases, extract it, and follow the bilingual first-run guide. GitHub's automatic source-code ZIP is not the product trial. A repository page alone does not mean a downloadable release exists.

## What you can do / 可以做什么

- Browser: load a built-in fictional example or an existing supported report, inspect coverage, and export a card as HTML/JSON. No Python is needed for this route.
- Python 3.10+: import an authorized report, slice or supported full-transaction `getBlock` JSON locally. No external Python packages are required.
- Optional free companion: `RADAR-权限阅读练习-中英社区包.zip` contains a separate token-permission reading exercise. It is not another paid product or the main workbench.

浏览器仅载入支持的研究报告；原始 getBlock 文件需走 Python 入口。工具不实时采集链上数据，也不判断代币安全、共同控制、开发者身份、买卖时机或收益。

## Trial scope / 试用范围

You may run the trial on your own device and read/export material you are entitled to use. The included original trial scope controls: no grant of paid resale, sublicensing or independent audit endorsement. This is not a general open-source licence, a paid release, a subscription or a promise of future updates or unlimited support. See the original scope inside the downloaded package (`使用范围.md`, and the original English scope where applicable).

工具不要求钱包连接、付款、持币或密钥。使用真实材料时，分享范围仍由原数据授权决定；导出可能含 mint、交易签名和共享账户标识。

## Feedback / 反馈

If you choose to try it, tell us the task, whether import/export worked, the blocking step, total minutes, and whether you would reuse it. Public feedback should omit private raw files, keys and customer records. The X brand account is [@radraw6o](https://x.com/radraw6o).

请反馈：想完成的任务、是否成功导入/导出、卡在哪一步、总用时、是否会再用。样例流程成功不等于真实用户采用或商业结果。
