## Context

見 proposal.md。這裡只寫跨專案選擇。各 repo 怎麼做寫在 `add-widget-lumen-*`。

## Goals / Non-Goals

**Goals:**

- 一個 JSON 欄位 `description` 從 API 經過 SDK 到消費端都看得到

**Non-Goals:**

- 持久化、認證、發套件、HTTP 重試
- 各 repo 的檔案怎麼切

## Decisions

- **在現有 `GET /widgets` 加 `description`，不另開 `GET /widgets/:id`。** 清單已經存在。否決：新的詳情 endpoint。
- **由 SDK 的 `widgetLabel` 組字串，不讓消費端自己拼。** 否決：只在 app 裡 concatenate。

## Risks / Trade-offs

- [沙盒用相對路徑 import SDK，repo 分開就會壞] → 沙盒接受；正式消費端會依賴已發佈的套件。路徑細節在 `add-widget-lumen-app`。
