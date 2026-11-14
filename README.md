# Sean Lin — 平面設計師作品集 Landing Page

自由接案平面設計師 Sean Lin 的個人作品集單頁網站（Landing Page），用來展示品牌識別、包裝與編輯設計作品，並提供聯繫方式。

## 網站功能

- **導覽列**：固定於頁面頂端（sticky）、毛玻璃效果，可快速跳至「作品」與「聯繫」區塊，並顯示「開放接案中」狀態。
- **英雄區塊（Hero）**：主標語、自我介紹、「與我聯繫／觀看作品」行動按鈕，以及經驗年數、完成專案、合作品牌等數據。
- **精選作品**：以卡片呈現三個代表專案（山嵐茶室、拾光咖啡 Roastery、城市漫遊 攝影展），包含類別、年份、說明與標籤。
- **頁尾聯繫區**：Email 聯繫按鈕（mailto）與社群連結（Behance、Instagram、Dribbble）。
- **淡入動畫**：區塊依序以 fade-up 動畫出現；若使用者系統開啟「減少動態效果」，會自動停用動畫（`prefers-reduced-motion`）。
- **RWD 響應式設計**：針對平板與手機（960px / 680px / 480px 斷點）調整版面、字級與卡片排列，手機上也能舒適瀏覽。

## 使用技術

- **HTML5**：語意化標籤（`nav`、`main`、`section`、`article`、`footer`）與 ARIA 標註。
- **CSS3**：CSS 變數（Custom Properties）、Grid / Flexbox 版面、漸層背景、`backdrop-filter`、`@keyframes` 動畫、Media Queries。
- **Google Fonts**：Inter 與 Noto Sans TC。
- 內嵌 SVG 圖示，無任何 JavaScript 或建置工具，所有樣式都寫在 `index.html` 中。

## 專案結構

```
claude-lab/
├── index.html   # 網站主頁（HTML + 內嵌 CSS）
└── README.md    # 專案說明
```

## 如何用瀏覽器開啟

不需要安裝任何套件，直接開啟 `index.html` 即可：

1. **直接雙擊**：在 Finder／檔案總管中找到 `index.html`，雙擊即會用預設瀏覽器開啟。
2. **使用終端機（macOS）**：
   ```bash
   open index.html
   ```
   Windows 可使用 `start index.html`，Linux 可使用 `xdg-open index.html`。
3. **（選用）本機伺服器**：
   ```bash
   python3 -m http.server 8000
   ```
   然後在瀏覽器開啟 <http://localhost:8000>。

> 想預覽手機版效果，可在 Chrome／Safari 開啟開發者工具，切換到裝置模擬模式（Chrome 快捷鍵：`Cmd + Shift + M`）。
