## Why

Widget 清單目前只有 `id` 與 `title`。跨 API、SDK、消費端要同一條產品行為：每個 widget 帶說明文字。

## What Changes

- `GET /widgets` 每個元素新增必填字串欄位 `description`
- Client SDK 提供 `widgetLabel(widget)`，把 title 與 description 組成一行
- 消費端列出 widget 時印出 `widgetLabel` 的結果

## Capabilities

### New Capabilities

- `widget`：跨 repo 的 widget 清單 JSON（`id`、`title`、`description`）。SDK 標籤與消費端列印分別在專案變更的 specs。

### Modified Capabilities

- （無）

## Impact

- lumen-api、lumen-sdk、lumen-app
- 專案變更：`add-widget-lumen-api`、`add-widget-lumen-sdk`、`add-widget-lumen-app`
