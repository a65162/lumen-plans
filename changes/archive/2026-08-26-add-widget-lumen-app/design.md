## Context

契約見產品規格變更 `add-widget`。本檔只寫 lumen-app 怎麼做。

## Goals / Non-Goals

**Goals:**

- 印 SDK 的 label；不在 app 裡自己組 title／description

**Non-Goals:**

- 改 API 或 SDK 介面

## Decisions

- **從 `../lumen-sdk/index.mjs` import `widgetLabel`。** 沙盒沒有發佈套件。否決：在 `app.mjs` 裡複製組字邏輯。

## Risks / Trade-offs

- [相對路徑在 repo 分開後會壞] → 沙盒接受。
