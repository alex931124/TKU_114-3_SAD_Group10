# 0714 User Stories & Acceptance Implementation

## 1. 小組與專案資料

- 課程名稱：系統分析與設計
- 日期：115/07/14
- 小組名稱：Group11
- 專案名稱：校園宿舍報修、派工與維修追蹤系統
- 組員與分工：張韡薺（需求整理、畫面驗收、文件整合）
- GitHub 儲存庫連結：本地工作區已建立 Git 記錄，未提供遠端儲存庫連結（待補上）
- 7/13 成果資料夾：../0713_Requirements_Code_Agent
- 0714 成果資料夾：./

## 2. 本次完成內容

本次選擇修正第一個可操作切片，重點為使原型在需求與驗收條件上可追溯、可操作、可驗收。

今日結果包含：
- 使用者故事清單
- 功能性需求清單
- 非功能性需求清單
- 業務規則、資料需求與限制條件
- 驗收條件
- 需求優先順序與品質檢查
- 實作待辦與更新後代理任務書
- 可操作切片修正與手動驗收紀錄
- 需求與畫面對照表與追溯矩陣

## 3. 如何開啟與操作

1. 以瀏覽器開啟 [../0713_Requirements_Code_Agent/first_working_slice/index.html](../0713_Requirements_Code_Agent/first_working_slice/index.html)
2. 於「宿舍學生」頁面填寫宿舍、房號、設備類型與問題描述後送出。
3. 切換到「宿舍管理員」頁面，選擇維修人員後點擊派工。
4. 切換到「維修人員」頁面，點「標記完成」以更新狀態。

## 4. 已通過與未通過的驗收條件

已通過：
- AC-01-01：學生可成功送出報修單
- AC-01-02：管理員可在清單中看見新增案件
- AC-02-01：管理員可派工給維修人員
- AC-02-02：維修人員可標記完成
- AC-NFR-01-01：必填欄位未填時不可送出

待確認/未完成：
- 重複報修辨識仍未納入本期範圍
- 正式登入、正式資料庫與通知未納入本期

## 5. 已知限制

- 本期僅使用前端假資料與 localStorage。
- 不包含正式單一登入、正式單一資料庫、金流、手機 App、採購流程。
- 需求包中的重複報修判斷已列為待確認問題。

## 6. 文件連結

- [user_stories.md](user_stories.md)
- [functional_requirements.md](functional_requirements.md)
- [non_functional_requirements.md](non_functional_requirements.md)
- [business_rules_data_constraints.md](business_rules_data_constraints.md)
- [acceptance_criteria.md](acceptance_criteria.md)
- [requirements_quality_review.md](requirements_quality_review.md)
- [requirements_priority.md](requirements_priority.md)
- [requirements_package_draft.md](requirements_package_draft.md)
- [traceability_matrix_draft.md](traceability_matrix_draft.md)
- [implementation_backlog.md](implementation_backlog.md)
- [updated_code_agent_brief.md](updated_code_agent_brief.md)
- [requirements_to_screen.md](requirements_to_screen.md)
- [manual_acceptance_test.md](manual_acceptance_test.md)
- [ai_code_agent_log.md](ai_code_agent_log.md)
- [evidence/](evidence/)

## 7. 本次提交紀錄

- 本地 Git 提交識別碼：3d04629
- 本次 0714 文件與修正版切片已放置於同一資料夾內。
