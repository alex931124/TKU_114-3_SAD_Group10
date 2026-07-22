# 需求文件包初稿（Requirements Package Draft）

## 1. 專案與範圍摘要

- 專案名稱：校園宿舍報修、派工與維修追蹤系統
- 本期核心範圍：報修提交、管理員派工、維修人員完成回報
- 本期範圍外：正式登入、正式資料庫、採購、金流、手機原生 App

## 2. 利害關係人與角色

- 宿舍學生：提交報修單與查看狀態
- 宿舍管理員：查看待處理清單並派工
- 維修人員：查看派工任務與標記完成
- 系統管理員：僅作後續擴充角色與權限預留，不在本期切片內實作

## 3. 需求來源表

- 主要來源：需求來源表（0713）
- 連結：../0713_Requirements_Code_Agent/requirements_source_table.md

## 4. 需求成果清單

- 使用者故事：見 [user_stories.md](user_stories.md)
- 功能性需求：見 [functional_requirements.md](functional_requirements.md)
- 非功能性需求：見 [non_functional_requirements.md](non_functional_requirements.md)
- 業務規則、資料需求與限制條件：見 [business_rules_data_constraints.md](business_rules_data_constraints.md)
- 驗收條件：見 [acceptance_criteria.md](acceptance_criteria.md)
- 需求優先順序：見 [requirements_priority.md](requirements_priority.md)

## 5. 需求追溯矩陣初稿

- 見 [traceability_matrix_draft.md](traceability_matrix_draft.md)

## 6. 未解決問題清單

- OI-01：是否需要額外重複報修判斷，並需補上來源與驗收條件。
- OI-02：角色權限是否只用前端切換即可，或需後續正式設計。
- OI-03：送出時間、派工時間與完成備註等資料欄位於本期是否須最小保存。

## 7. 版本與變更紀錄

| 版本 | 日期 | 變更內容 | 變更原因 |
| --- | --- | --- | --- |
| 0.1 | 115/07/14 | 需求文件包初稿建立 | 將 7/13 需求來源整理成可追溯需求包 |
| 0.2 | 115/07/14 | 修正驗收與優先順序細節 | 讓需求可用於切片實作與手動驗收 |
