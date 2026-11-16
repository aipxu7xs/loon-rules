# loon-rules

Loon 远程规则仓库，由 Muse 为 sksn 维护。规则文件只写域名/IP，不写策略；策略在 Loon 里订阅时选择，以后更新 GitHub 上的文件，Loon 端会自动更新。

## LINE.list

让 LINE 走香港节点（账号绑定 +852 香港号码，地区要对上）。

订阅地址（raw）：
https://raw.githubusercontent.com/aipxu7xs/loon-rules/main/LINE.list

在 Loon 里添加：
1. 打开 Loon → 配置 → 规则 → 远程规则 → 添加
2. URL 粘贴上面的 raw 地址
3. 策略（policy）选择香港Auto
4. 标签（tag）写 LINE，启用

## USAI.list

美国 AI 补充名单：Kelee 的 AI.lsr 没覆盖到的美国 AI 服务（Poe、Character.AI、Midjourney、Runway、Suno、ElevenLabs、Hugging Face、Cursor、Replicate、Luma、Pika、HeyGen、You.com），统一走美国节点。

订阅地址（raw）：
https://raw.githubusercontent.com/aipxu7xs/loon-rules/main/USAI.list

添加方式同上，策略（policy）选择美国Auto，标签（tag）写 USAI。

## BING.list

必应全家（bing.com / bingapis.com / bing.net / bing.com.cn）统一走香港节点。原因：必应原本被拆开 — www.bing.com 被 AI 规则带去美国、其余子域名被微软规则带去基础代理，两个出口地区导致必应老报“网络出现问题”。此表在配置里排在 AI 规则之前，先命中先赢。

订阅地址（raw）：
https://raw.githubusercontent.com/aipxu7xs/loon-rules/main/BING.list

添加方式同上，策略（policy）选择香港Auto，标签（tag）写 Bing。
