# 山东金宇9月调价对比

基于《山东金宇9月电价调整.xlsx》整理，覆盖金宇及 5 个周边场站、10 个统一时段、50 组价差。

GitHub 页面会自动解压并校验完整交互页面。离线使用请打开单文件版《山东金宇9月调价对比.html》。支持选择参考场站、调整定价策略、逐时段修改价格、切换总价/电费/服务费价差、导出 CSV。在线修改后可复制浏览器地址分享当前方案。

## 发布为 HTTPS 页面

将 index.html、payload-0.txt 至 payload-3.txt 与 .nojekyll 放在仓库根目录。进入 Settings → Pages，在 Source 选择 Deploy from a branch，Branch 选择 main，Folder 选择 /(root)，点击 Save。页面部署后，使用 Pages 页面显示的网址分享。

GitHub 官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 计算口径

价差 = 山东金宇价格 − 对比场站价格，正值表示金宇更贵。按原表实际开始/结束时间对齐，全日末尾 23:59 按 24:00 衔接。电费与服务费独立核对。价格单位按元/度理解。

默认策略为只降不涨、匹配已选场站最低总价，并保持原电费不变。平段总价 0.78，11:00–14:00 总价 0.38，其他时段保持原总价。该方案为模拟，未应用到实际场站。

数据为本次提供表格的固定快照，未包含充电量、成本、促销或收益预测。
