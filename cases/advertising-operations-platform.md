# 广告运营数据平台

角色：需求梳理、数据平台设计与本地部署

## 背景

Meta、Google 与 Shopify 数据分散，经营口径不统一，运营分析依赖多平台切换和人工整理。

## 关键工作

- 主动学习广告运营口径，将沟通内容整理为分阶段 PRD 与只读优先的安全边界
- 搭建 Airbyte、PostgreSQL、Metabase 本地数据底座及备份恢复链路
- 将 Shopify 经营真值与 Meta 投放归因分开展示，避免跨平台收入重复相加
- 建立 Campaign、Ad Set、Ad 与 Creative 下钻视图，为后续受控广告操作和 AI Skills 预留接口

## 结果

- 完成 试点业务单元 经营快照与 试点业务单元 Meta 投放诊断两套只读看板的数据基础。
- Meta Insights 已落库 23,650 条唯一广告日记录，覆盖 2024-08-14 至 2026-08-14。

技术：Airbyte、PostgreSQL、Metabase、Docker、WSL 2、ShopifyQL、Meta Marketing API、SQL
