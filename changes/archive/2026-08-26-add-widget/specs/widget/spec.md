## Purpose

定義跨 repo 的 widget 清單 JSON：每個元素有 `id`、`title`、`description`。

## ADDED Requirements

### Requirement: Widget 清單含 description
API MUST 接受 `GET /widgets` 並回應狀態 200。本體 MUST 為 JSON 陣列。每個元素 MUST 為物件，且有字串欄位 `id`、`title`、`description`。種子資料 MUST 使用 id `w-1`、title `Demo widget`、description `Sandbox widget`。

#### Scenario: 種子 widget 有 description
- **WHEN** 客戶端送出 `GET /widgets`
- **THEN** 回應狀態為 200，JSON 陣列含一個物件，其 `id` 為 `w-1`、`title` 為 `Demo widget`、`description` 為 `Sandbox widget`
