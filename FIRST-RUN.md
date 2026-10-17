# 第一次使用 / First run

本说明面向完整的 `RADAR-链上研究证据工作台-0.3.4-候选.zip`，不是权限阅读社区包，也不是 GitHub 自动生成的源码 ZIP。请先完整解压到新文件夹。

## 中文：先导出一张虚构卡片

1. 在解压后的主包目录打开 `research-review.html`。
2. 点击 **载入虚构示例**。第一次练习到这里不需要选择 JSON，也不需要第二份报告。
3. 查看窗口 **3 / 4**、已观察共现交易 **1**、共享账户 **1**、元数据不全 **1**。这是内置的部分覆盖样例；不是完整历史，更不代表真实代币风险。
4. 点击 **下载第一份卡片 HTML**。打开下载的 `RADAR-虚构研究卡.html`；想保留结构化结果时，再点 **下载第一份卡片 JSON**，得到 `RADAR-虚构研究卡.json`。
5. 看到导出的卡片仍写明虚构演示、覆盖与未知项，即完成这次练习。点击 **清除** 可移除页面内存中的卡片；已下载文件仍保留。

浏览器页面需启用 JavaScript。页面以本地文件使用；如果你的浏览器或设备策略不允许打开、下载，请记录具体阻点，不要关闭安全保护。此说明核对了页面按钮与代码路径；特定设备的 file 协议行为需在该设备确认。

### 第二次练习（可选）

使用页面第一份报告的文件选择器，选择主包的 `examples/fictional-partial.json`，观察覆盖和未知项如何变化。这是另一次练习，不是内置样例导出的必要步骤。网页不能直接导入 `fictional-getblock-*.json` 原始区块文件。

### Python 路线（可选）

在已解压主包目录打开终端，需要 Python 3.10 或更新版本。输出目录 `my-first-card` 必须尚不存在。

```sh
python3 research_card.py --slice examples/fictional-slice.json --output my-first-card
```

打开 `my-first-card/card.html`。同目录还生成 `card.json` 和 `engine-report.json`；后者可导入网页。这个切片样例与浏览器内置样例不同，不应要求数值完全相同。

## English: export your first fictional card

1. In the fully extracted product folder, open `english/research-review.html`. `english/START-HERE.html` provides an additional guided report exercise.
2. Click **Load synthetic example**. Do not select a file or a second report for this first exercise.
3. Expect a window of **3 / 4**, **1** observed co-occurring attempt, **1** shared account and **1** incomplete neighbor. The example is fictional and has partial coverage.
4. Click **Download first card as HTML** and open `RADAR-synthetic-research-card.html`. The JSON button saves `RADAR-synthetic-research-card.json`.
5. Confirm that the exported card retains the fictional-data notice and evidence limits. **Clear** removes the in-memory card, not files already downloaded.

JavaScript must be enabled. Device/browser policies may limit local-file opening or downloading; report a specific blocker rather than weakening security settings. Python is not needed for the browser exercise.

For an optional CLI exercise, run the command above from the extracted package with Python 3.10+ and a new output directory. Open `my-first-card/card.html`, or load its `engine-report.json` into the browser viewer. Raw getBlock JSON requires the Python `--block` route documented in the product README.

## What counts as finishing / 完成标准

You opened the tool, inspected the synthetic report, exported a card and could reopen it with its limits intact. This confirms a sample workflow only. It does not establish live chain verification, complete history, common control, asset safety, customer adoption or income.

自愿反馈可以只提供：任务 / task；完成的步骤 / completed step；阻点 / blocker；总分钟 / total minutes；是否会再用及用途 / reuse and purpose。不要为反馈提供密钥或私有原始资料。
