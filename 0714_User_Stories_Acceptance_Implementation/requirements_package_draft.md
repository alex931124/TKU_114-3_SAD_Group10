# 需求文件包初稿（Requirements Package Draft）

## 1. 專案與範圍摘要

- 專案名稱：校園宿舍報修、派工與維修追蹤系統
- 本期核心範圍：報修提交、管理員派工、維修人員完成回報
- 本期範圍外：正式登入、正式資料庫、採購、金流、手機原生 App
- 本次交付目的：將需求來源轉為可追溯、可驗收、可實作的文件包，並修正第一個可操作切片

## 2. 利害關係人與角色

| 角色 | 主要目的 | 本期關注程度 |
| --- | --- | --- |
| 宿舍學生 | 提交報修單並查看狀態 | 高 |
| 宿舍管理員 | 查看待處理清單並派工 | 高 |
| 維修人員 | 查看派工任務並完成回報 | 高 |
| 系統管理員 | 後續權限管理預留角色 | 中 |

## 3. 需求來源資訊

- 主要來源：0713 需求來源表
- 來源文件：../0713_Requirements_Code_Agent/requirements_source_table.md
- 來源強度主要集中於訪談與專案章程，確保需求不由 AI 推測自行增加

## 4. 需求成果索引

- 使用者故事：見 [user_stories.md](user_stories.md)
- 功能性需求：見 [functional_requirements.md](functional_requirements.md)
- 非功能性需求：見 [non_functional_requirements.md](non_functional_requirements.md)
- 業務規則、資料需求與限制條件：見 [business_rules_data_constraints.md](business_rules_data_constraints.md)
- 驗收條件：見 [acceptance_criteria.md](acceptance_criteria.md)
- 需求品質檢查：見 [requirements_quality_review.md](requirements_quality_review.md)
- 需求優先順序：見 [requirements_priority.md](requirements_priority.md)
- 需求追溯矩陣：見 [traceability_matrix_draft.md](traceability_matrix_draft.md)

## 5. 需求追溯重點

本次文件包已將以下鏈路補齊：

- 來源編號 → 使用者故事 → 功能性需求 / 非功能性需求
- 功能性需求 → 驗收條件 → 視覺畫面與操作
- 驗收條件 → 手動測試紀錄與證據影像

這樣可以避免後續只看到最後畫面，卻無法知道需求來源與對應驗收標準。

## 6. 未解決問題清單

| 問題編號 | 問題 | 說明 |
| --- | --- | --- |
| OI-01 | 重複報修辨識 | 目前需求來源中僅有候選項目，未在本期直接實作 |
| OI-02 | 角色權限正式化 | 本期用角色切換做簡化顯示控制，尚未正式建立權限系統 |
| OI-03 | 資料欄位最小保存範圍 | 送出時間、派工時間與完成備註是否要正式保存，待下一階段確認 |

## 7. 版本與變更紀錄

| 版本 | 日期 | 變更內容 | 變更原因 |
| --- | --- | --- | --- |
| 0.1 | 115/07/14 | 建立需求文件包初稿 | 將 7/13 需求來源整理成可追溯成果 |
| 0.2 | 115/07/14 | 補強驗收條件、優先順序與手動驗收紀錄 | 讓需求可直接對應切片與操作驗收 |
| 0.3 | 115/07/14 | 整理為 GitHub 可讀版提交格式 | 提升文件可閱讀性與交付品質 |

## 8. 結論

本需求文件包目前已具備「需求來源 → 使用者故事 → 功能性需求 → 驗收條件 → 手動測試」的可追溯骨架，適合作為下一階段使用案例與使用情境課程的基礎文件。
