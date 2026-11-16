# loon-rules

Loon 远程规则仓库，由 Muse 为 sksn 维护。规则文件只写域名/IP，不写策略；策略在 Loon 里订阅时选择，以后更新 GitHub 上的文件，Loon 端会自动更新。

## LINE.list

让 LINE 走日本节点，解决 LINE 登录走错节点的问题。

订阅地址（raw）：
https://raw.githubusercontent.com/aipxu7xs/loon-rules/main/LINE.list

在 Loon 里添加：
1. 打开 Loon → 配置 → 规则 → 远程规则 → 添加
2. URL 粘贴上面的 raw 地址
3. 策略（policy）选择你的日本节点/日本策略组
4. 标签（tag）写 LINE，启用
5. 保存后重启 Loon，LINE 强退后重新登录
