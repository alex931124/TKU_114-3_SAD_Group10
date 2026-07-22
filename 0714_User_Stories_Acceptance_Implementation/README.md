# 0714 User Stories & Acceptance Implementation

## 1. 專案摘要

本次提交聚焦於將 7/13 的需求來源整理成可追溯、可驗收、可實作的需求文件包，並修正第一個可操作切片，使其能完成從「學生報修」到「管理員派工」再到「維修人員完成回報」的核心流程。

本次選擇的方式是：修正第一個可操作切片，而非擴充新功能。

## 2. 小組與專案資料

- 課程名稱：系統分析與設計
- 日期：115/07/14
- 小組名稱：Group11
- 專案名稱：校園宿舍報修、派工與維修追蹤系統
- 組員與分工：張韡薺（需求整理、畫面驗收、文件整合）
- 7/13 成果資料夾：../0713_Requirements_Code_Agent
- 0714 成果資料夾：./
- GitHub / 版本管理狀態：本地 Git 已完成提交；遠端倉庫連結待補上

## 3. 本次交付內容

本次交付包含以下成果：

- 使用者故事清單
- 功能性需求清單
- 非功能性需求清單
- 業務規則、資料需求與限制條件
- 驗收條件
- 需求品質檢查與衝突紀錄
- 需求優先順序
- 需求文件包初稿
- 實作待辦清單
- 更新後的程式碼代理實作任務書
- 需求與畫面對照表
- 手動驗收測試紀錄
- 生成式 AI / 程式碼代理使用紀錄

## 4. 本次選擇的實作方向

### 修正第一個可操作切片

目標是改善原型使其能更明確對應需求與驗收條件，重點不在新增功能，而是讓目前流程可以更穩定地完成：

1. 學生可提交報修單
2. 管理員可查看新增案件並派工
3. 維修人員可完成回報
4. 必填欄位驗證可防止資料缺漏

## 5. 如何開啟與操作

1. 以瀏覽器開啟原型：
   - [../0713_Requirements_Code_Agent/first_working_slice/index.html](../0713_Requirements_Code_Agent/first_working_slice/index.html)
2. 切換到「宿舍學生」角色，填寫宿舍、房號、設備類型與問題描述後送出。
3. 切換到「宿舍管理員」角色，查看待處理清單並選擇維修人員派工。
4. 切換到「維修人員」角色，點選「標記完成」更新案件狀態。

## 6. 驗收狀態摘要

### 已通過

- AC-01-01：學生可成功送出報修單
- AC-01-02：缺少必填欄位時不可送出並顯示錯誤訊息
- AC-02-01：管理員可看到新增案件並派工
- AC-02-02：維修人員可完成回報並更新狀態
- AC-NFR-01-01：表單必填驗證與中文錯誤提示可操作檢查

### 待確認 / 本期未納入

- 重複報修辨識尚未納入本期實作
- 正式登入、正式資料庫、採購、金流、手機原生 App 均屬本期範圍外

## 7. 已知限制

- 本期僅使用前端假資料與 localStorage
- 不包含正式單一登入與正式資料庫
- 不包含外部通知、採購與付款流程
- 重複報修判斷已列為待確認問題，未在本期擴增功能

## 8. 文件索引

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

## 9. 驗證與提交紀錄

本次已完成本地版本提交，驗證結果如下：

- 提交訊息：docs: 完成使用者故事與需求文件包初稿
- 提交識別碼：dd4fb8e

驗證證據保存在以下位置：

- [manual_acceptance_test.md](manual_acceptance_test.md)
- [evidence/](evidence/)

## 10. 結論

本次 0714 需求整理與切片修正成果已完成，文件與實作可用於後續 7/20 的使用案例與使用情境延伸。此版本保持範圍控制，避免把程式碼代理或原型擴張成完整宿舍管理系統。
