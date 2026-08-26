## Why

在 lumen-sdk 落地產品規格 `add-widget`，並提供組標籤的 helper。

## What Changes

- 匯出 `widgetLabel(widget)`，回傳 `{title} — {description}`
- `listWidgets` 仍回傳 API 的 JSON 陣列（含 `description`）

## Capabilities

### New Capabilities

- `widget-label`：SDK `widgetLabel` 的字串契約

### Modified Capabilities

- （無）

## Impact

- 僅 lumen-sdk
- 產品規格變更：`add-widget`
