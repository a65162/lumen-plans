## Purpose

定義 Client SDK 如何把 widget 的 title 與 description 組成一行標籤字串。

## ADDED Requirements

### Requirement: SDK 組成 widget 標籤
`widgetLabel(widget)` MUST 回傳字串 `{title} — {description}`，使用該 widget 的 `title` 與 `description`，中間為空白、em dash、空白。

#### Scenario: 標籤接上 title 與 description
- **WHEN** 以 `{ title: "Demo widget", description: "Sandbox widget" }` 呼叫 `widgetLabel`
- **THEN** 回傳值為 `Demo widget — Sandbox widget`
