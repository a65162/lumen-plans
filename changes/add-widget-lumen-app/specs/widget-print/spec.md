## Purpose

定義消費端列出 widget 時印出什麼：每一行必須是 SDK `widgetLabel` 的回傳值。

## ADDED Requirements

### Requirement: App 印出 SDK 標籤
app 的列表命令 MUST 每個 widget 印一行。每一行 MUST 正好是該 widget 經 `widgetLabel` 得到的字串。

#### Scenario: App 那一行符合 SDK 標籤
- **WHEN** 對種子 API 執行 app 列表命令
- **THEN** stdout 含有一行 `Demo widget — Sandbox widget`
