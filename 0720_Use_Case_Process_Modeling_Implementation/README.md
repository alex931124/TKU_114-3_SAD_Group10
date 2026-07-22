# 0720 使用案例與流程模型化實作交付

## 分析範圍

本次分析緊扣 0714 需求文件包初稿與第一個可操作切片，聚焦校園宿舍報修、派工與維修追蹤系統三個核心角色：

- 宿舍學生：提交報修需求
- 宿舍管理員：查看待處理清單並派工
- 維修人員：查看已派工任務並完成回報

## 主要參與者與使用案例

| 角色 | 核心使用案例 |
| --- | --- |
| 宿舍學生 | 提交報修、查看報修狀態 |
| 宿舍管理員 | 查看待處理清單、派工 |
| 維修人員 | 查看已派工任務、完成維修 |

## 現況問題與目標改善摘要

| 痛點 | 現況狀態 | 目標改善 |
| --- | --- | --- |
| 報修資訊分散 | 學生透過電話或訊息回報 | 統一報修入口 |
| 清單不集中 | 管理員要人工整理訊息 | 待處理清單集中顯示 |
| 狀態不可視 | 學生無法即時知道進度 | 狀態標籤與流程可追蹤 |

## 本次實作選擇與操作方式

本次實作採用「修正既有切片」方式，延續第一個可操作切片的三角色介面與前端假資料存儲方式。

操作步驟：
1. 在瀏覽器開啟 [revised_or_third_working_slice/index.html](revised_or_third_working_slice/index.html)
2. 以宿舍學生角色送出報修表單
3. 切換到宿舍管理員角色，檢查待處理清單並派工
4. 切換到維修人員角色，標記完成

## 已通過與未通過驗收條件

### 已通過
- AC-01-01：學生成功送出報修並顯示案件編號與狀態
- AC-02-01：管理員可查看待處理清單
- AC-02-02：管理員可派工給維修人員
- AC-03-01：維修人員可查看已派工任務
- AC-03-02：維修人員可完成回報
- AC-NFR-01-01：必填欄位空白時可阻止送出

### 待確認 / 未納入
- AC-02-03：未選擇維修人員時的保護行為
- AC-03-03：重複點擊完成時的去重保護
- 重複報修辨識（OI-01）

## 已知限制與待確認問題

- 本期仍使用前端角色切換模擬權限，不是正式登入系統。
- 實作只保存假資料，沒有正式資料庫與後端。
- 重複報修識別、送出時間紀錄與完整權限管理待後續需求確認。

## 成果連結

- 角色目標矩陣：[actor_goal_matrix.md](actor_goal_matrix.md)
- 使用案例清單：[use_case_inventory.md](use_case_inventory.md)
- 使用案例描述：[use_case_descriptions.md](use_case_descriptions.md)
- 現況與目標流程對照：[process_problem_improvement.md](process_problem_improvement.md)
- 流程資料交換：[process_data_exchange.md](process_data_exchange.md)
- 模型一致性矩陣：[model_consistency_matrix.md](model_consistency_matrix.md)
- 實作待辦：[implementation_backlog.md](implementation_backlog.md)
- 更新後程式碼代理任務書：[updated_code_agent_brief.md](updated_code_agent_brief.md)
- 手動驗收測試：[manual_acceptance_test.md](manual_acceptance_test.md)
- AI 使用紀錄：[ai_code_agent_log.md](ai_code_agent_log.md)

## 本次提交紀錄

- 目前工作區尚未建立正式 Git commit，可先以本地資料夾提交。
- 建議提交訊息：`新增 0720 Use Case 與 Process Modeling 交付文件`
