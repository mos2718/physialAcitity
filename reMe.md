# 
## 提問範例

### 建立 documentReference
若在 FHIR documentReference 當中存放的是規格文件，如 MD 檔、JSON 檔、或 CSV  檔，且清楚記錄文件類別、編號、版本、發布時間、作者、管理者，需要那些欄位


若 FHIR server 為 https://hapi.fhir.org/baseR4
請提供一可產生 FHIR documentReference 的 HTML 網頁程式，HTML、JS、CSS 寫在一起，使用單純的 JS 與法，儘量簡單之 CSS， 
程式可自動產生 UUID 當作 Practitioner 的 ID，
作者
"resourceType": "Organization",
  "id": "b3bf1db5-e176-4a8d-b0e6-7bff291894b0"

程式可自動產生 UUID 當作 Practitioner 的 ID，
可輸入暱稱及專業，button 點選後，產生及 put FHIR Practitioner，並將回應結果呈現。

