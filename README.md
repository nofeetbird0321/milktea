# 少喝一杯 · 独立域名版

目标地址：https://tea.nofeetbird.tech/

纯 HTML / CSS / JavaScript，无后端或第三方依赖。每次没买奶茶时记下金额，查看月度、年度与历年累计；提供 JSON 备份导出与合并导入。

## GitHub Pages

独立仓库目标为 `nofeetbird0321/milktea`，站点文件放在发布分支根目录。Pages 使用分支根目录发布，Custom domain 为 `tea.nofeetbird.tech`，启用 Enforce HTTPS。

Cloudflare DNS 配置：CNAME，名称 `tea`，目标 `nofeetbird0321.github.io`，DNS only，TTL Auto。先配置 GitHub Pages 的 Custom domain，再写入 DNS。

原工具箱 `tools.nofeetbird.tech` 保留，旧奶茶账本路径 https://tools.nofeetbird.tech/milktea/ 保留，以便导出旧记录。

## 数据迁移

新旧域名各自拥有独立的浏览器本地存储，不会自动共享记录。

1. 用曾记过账的设备和浏览器打开旧地址。
2. 点“备份与迁移”，导出全部记录的 JSON 文件。
3. 打开新地址，点“备份与迁移”，导入刚才的文件。
4. 检查年度累计与记录数。导入会合并，重复编号不会再次计入。

不要提前清除旧域名的网站数据。记录金额代表未消费金额，不代表实际银行存款。

## 发布状态

本文件描述待执行的独立域名配置；是否完成以 `deployment.json` 的实时验证结果为准。
