# RADAR Research Evidence Workbench

Turn supported Solana research JSON into shareable evidence cards, on your own device.

**[Download the free 0.3.4 local trial](https://github.com/xhwm41319-a11y/radar-workbench/releases/tag/v0.3.4)** · **[First-run guide](https://github.com/xhwm41319-a11y/radar-workbench/blob/v0.3.4/FIRST-RUN.md)** · **[Package checksums](https://github.com/xhwm41319-a11y/radar-workbench/blob/main/SHA256SUMS.txt)**

## What you can do

- Open the browser workbench, load its built-in fictional example or a supported research report JSON, and export a self-contained HTML or JSON card.
- Review the reported observation window, co-occurring transaction attempts, shared writable accounts, missing data and evidence limits in one place.
- Use the optional Python command line to calculate a report from a supported local slice or documented `getBlock` JSON export (`transactionDetails: full`). It reads your file; it does not fetch a block.
- Compare two compatible reports. When identifiers, versions, filters or coverage differ, the workbench keeps observations separate instead of implying a meaningful numeric change.

This is a file-based research review tool. The 0.3.4 download does not stream live RPC events, issue whale alerts, inspect Token-2022 contract bytecode or determine whether a token is safe. It does not connect a wallet, submit transactions or establish profitability.

## Export your first card

1. Download the research workbench archive from the release page and extract it completely.
2. Open `research-review.html` for Chinese, or `english/research-review.html` for English.
3. Click **载入虚构示例 / Load synthetic example**. No Python, input file or second report is needed for this exercise.
4. Expect window coverage **3 / 4**, observed co-occurring attempts **1**, shared accounts **1**, and missing / incomplete neighbors **0 / 1**.
5. Click **下载第一份卡片 HTML / Download first card as HTML** and open the downloaded card.

All built-in example identifiers and transactions are fictional. The downloaded card retains that notice and the coverage limits. Local-file opening and downloads remain subject to your browser settings.

## Bring your own material

| Input | Entry |
|---|---|
| Supported RADAR offline report or Co-occurrence Explorer 1.2.2 report JSON | Browser report selector or Python `--report` |
| Supported local slice | Python `--slice` |
| Documented `getBlock` JSON / jsonParsed file (`transactionDetails: full`), legacy/v0/v1 | Python `--block`, following the included format guide |

The browser selector does **not** accept arbitrary block responses, token addresses or wallet CSVs. Use the included CLI instructions for supported raw block exports. The format setting does not verify the source or completeness of an exported file. A sample report command is:

```sh
python3 research_card.py --report examples/fictional-report.json --output my-report-card
```

Python 3.10+ standard library is needed only for the CLI. Choose a new output directory; then open `my-report-card/card.html`. The browser interface has no npm build step or external JavaScript dependency. The download release is 0.3.4; generated-card metadata and browser assets retain version 0.3.3.

## Evidence boundaries

Counts describe the supplied material and declared window. Source authenticity, complete chain history, common control, developer attribution, Jito bundles, asset safety and trading returns are not established. Failed transaction attempts may be included; partial coverage produces observed lower bounds. The input's claimed slot is not an independent chain verification.

The released processing code works locally without a live data provider. Links to GitHub or community pages are external websites. This release provides no comparative latency benchmark against trading dashboards or bots; no latency advantage is established.

## Trial scope and feedback

The release contains source files for inspection and local use under its included usage-scope files (`使用范围.md`; `english/TRIAL-SCOPE-original.md` preserves the Chinese original). Those trial terms do not grant paid resale or sublicensing; this README does not replace them or grant an Apache-2.0 license.

For voluntary feedback, tell us the task, input format, blocking step, whether you exported a usable card, time spent and whether you would use it again. Keep private keys, API keys and unauthorized customer or raw research files out of public reports.

[Research community](https://t.me/sol_alpha_radar_lab) · [Brand updates](https://x.com/radraw6o)

---

## 中文

RADAR研究证据工作台用于把**已有、受支持的Solana研究JSON**整理为可保存和分享的证据卡。它适合复核报告中的覆盖、共现、共享账户及未知项；减少整理步骤的实际工时收益仍待使用反馈验证。

浏览器先用内置虚构示例即可导出第一张卡，不需要Python、钱包或第二份报告。原始getBlock文件须按包内格式说明走Python入口，不能直接拖入网页。当前下载包不提供实时行情、鲸鱼预警或恶意代币判定，也不证明输入来源真实、代币安全或收益。

当前为免费本地试用，使用及再分发范围以包内原文为准。研究包与社区练习包在发行页分别列出；其他内部原型或Bot的功能不属于本发行附件。
