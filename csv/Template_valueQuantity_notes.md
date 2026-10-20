# Template.json 與 diff.csv 欄位映射

1. 依 `activity_code` 篩選 CSV。
2. ADL/IADL 類活動：顯示 `result_display_zh`，選取後將同列 `value`、`unit`、`unit_system`、`unit_code` 寫入 `Observation.valueQuantity`。
3. 數值型測試／感測：顯示數值輸入欄位，輸入值取代 CSV 空白的 `value`，單位由該活動列取得。
4. 調閱時，依 `activity_code` + `valueQuantity.value` 查回分級列，取得 `result_code` 與多語顯示。
5. `valueQuantity.value` 必須是 JSON number，不可作為字串送出。
6. 不把「未評估／未完成」寫成 0 或其他分數；沒有觀察值時，不建立該 Observation。
7. `valueQuantity` 不承載左右側、測試條件、統計期間或裝置來源；如有需要，Micro-IG 應另訂欄位映射。
