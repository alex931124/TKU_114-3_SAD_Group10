# 實作待辦清單（Implementation Backlog）

| 待辦編號 | 需求與驗收條件 | 工作內容 | 影響範圍 | 前置依賴 | 完成標準 | 驗證方式 | 優先順序 | 狀態 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| IMP-01 | FR-01、AC-01-01、AC-01-02 | 製作報修表單與必要欄位驗證 | index.html、style.css、script.js | 無 | 可填寫並成功送出，空欄不可送出 | MAT-01、MAT-02 | 1 | 已完成 |
| IMP-02 | FR-02、AC-01-03 | 顯示報修成功狀態與案件編號 | script.js、studentResult 區塊 | IMP-01 | 送出後可看到「已提交」與案號 | MAT-03 | 2 | 已完成 |
| IMP-03 | FR-03、AC-02-01 | 管理員清單呈現與派工操作 | managerPanel、script.js | IMP-01 | 可查看新案件並指定維修人員 | MAT-04 | 3 | 已完成 |
| IMP-04 | FR-04、AC-02-02 | 更新派工後狀態為「已派工」 | script.js、managerList | IMP-03 | 派工後狀態與人員更新一致 | MAT-05 | 4 | 已完成 |
| IMP-05 | FR-05、AC-03-01 | 維修人員任務列表顯示 | technicianPanel、script.js | IMP-04 | 已派工案件可在維修清單中顯示 | MAT-06 | 5 | 已完成 |
| IMP-06 | FR-06、AC-03-02 | 維修完成回報 | technicianPanel、script.js | IMP-05 | 點擊完成後可顯示「已完成」 | MAT-07 | 6 | 已完成 |
