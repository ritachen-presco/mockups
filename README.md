# mockups

研究/發想階段要分享的 UI mockup(原型)。**GitHub Pages 託管 + PageCrypt 加密**。

> ⚠ **本 repo 只放「加密後」的檔案。明文原始 mockup 絕不進來**(明文進 git = 保護失效)。明文原始檔留在研究區 Drive 該構想夾。

## 做法(對齊 `G:\我的雲端硬碟\Projects-Research\README.md` 的 Mockup 分享)
- **建構**:每個 mockup = **單一自包含 HTML + JS 切畫面**(全內聯、圖用 SVG/壓縮)。不要多檔互連。
- **加密**:`npx pagecrypt <明文>.html <輸出>.html <密碼>` → 只把**輸出(密文)**放進本 repo。
- **每專案一組密碼**;密碼記在**研究區私人筆記** `_mockup-密碼對照(私人).md`(**不進本 repo**)。
- **發布**:push → GitHub Pages 服務 → 給 `URL + 密碼`。
- **換/撤銷**:重加密 + 覆蓋同檔 + push。

## 結構
```
mockups/
  <專案>/index.html      ← 加密後的單檔 mockup
  .nojekyll              ← 讓 Pages 直接服務靜態檔
```
URL 形如:`https://ritachen-presco.github.io/mockups/<專案>/index.html`

## 安全提醒
- PageCrypt = 客戶端 AES,擋一般人夠;用**強 passphrase**;高敏感內容評估改用 Cloudflare Access。
- 公開 repo OK —— 因為裡面全是密文。
