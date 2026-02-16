# andyuan2

自用 OpenClash 分流规则（`prokiki.ini`）。

## 最近调整（2026-02-17）

- 统一 dler 规则源到 `raw.githubusercontent.com`，降低订阅更新失败概率。
- 修复日本节点正则乱码（`埼玉`）。
- 合并多组手动切换为单组 `🐸 手动切换`，简化维护。
- 健康检查 URL 统一改为 HTTPS：`https://www.gstatic.com/generate_204`。
- 优化美国节点/故转匹配精度，减少误命中。
- 降低部分重叠规则：
  - 注释 `GoogleCN.list`（保留 Google 主规则）
  - 注释 `Domestic IPs.list`（由 `GEOIP,CN` 覆盖）
- 增加 `prokiki.ini` 结构化注释，便于长期维护。

## 使用方式

在 OpenClash 订阅转换模板中引用：

- `https://raw.githubusercontent.com/prokiki/andyuan2/main/prokiki.ini`

更新订阅后，应用配置即可。


## 备注

- 已注释的候选规则/策略已迁移到 `prokiki.disabled.ini` 备用。
