README — 前端原型 (PBI p00006)

## 目的

此 README 針對 `p00006_quick_prototype`（前端原型）提供快速啟動與展示說明。原型為 `Vite + Vue` 切片，透過單頁應用與 JSON 假資料展示核心使用者流程。

## 快速啟動

1. 進入專案根目錄。
2. 啟動 Vite 開發伺服器（PowerShell 範例）：

```powershell
Set-Location -Path "f:\se\rental-information-aggregation-platform\frontend\prototype"
npm install
npm run dev
# (或) Start-Process "http://localhost:5173/"
```

3. 在瀏覽器開啟 Vite 提示的本機網址（通常是 `http://localhost:5173/`）開始操作。

## 使用指引

- 登入（模擬）：使用 fixtures 中的使用者資料登入；session 在 localStorage 中保存。
- 房源列表：以 Vue 元件呈現，可使用關鍵字/城市/租金區間進行 client-side 篩選與分頁。
- 房源明細：查看完整費用揭露欄位（租金、押金、管理費、計費基準等）。
- 訊息：在訊息頁與房源明細中模擬發送訊息；訊息僅存在於記憶體/localStorage 中。

## 技術債與注意事項

- 本原型僅為 UI/UX 驗證用途，無任何後端持久化或安全保證。
- 若需與後端整合，建議同時建立 API PBI（p00007）並標準化端點/請求格式。

## Vite 開發環境

- 建議以 `npm run dev` 啟動 Vite，並在 `package.json` 中定義 `dev` / `build` / `preview` 指令。
- Vite 會提供熱重載與更順暢的 Vue 開發體驗，且不需要 Python。

## 後續工作建議

- 完成 fixtures 與 UI 綁定之後，若需要串接後端，可將部分資料來源改成 mock API 或直接接正式 API。
