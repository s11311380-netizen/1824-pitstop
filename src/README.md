# src/ 模組目錄 (Module Directory)

這裡是專案的原始碼模組預留目錄。團隊成員可以依據功能分工在此建立個別 JavaScript 檔案，並在 `index.html` 中引入。

---

## 建議模組分工

| 模組檔案 | 負責功能建議 | 說明 |
| :--- | :--- | :--- |
| `src/player.js` | 玩家角色管理 | 玩家外觀、屬性、操控移動邏輯 |
| `src/obstacles.js` | 障礙物與生成器 | 路上障礙物/車輛的隨機生成、下落邏輯與碰撞判定 |
| `src/game.js` | 遊戲狀態與計分 | 開始、暫停、Game Over 判定、分數計算與顯示 |
| `src/audio.js` | 音效與背景音樂 | 引擎聲、碰撞音效、得分音效 |

---

## 如何引入模組？

在根目錄的 `index.html` 底部的【組員引入模組預留位置】標籤下方新增 script 標籤：

```html
<script src="src/obstacles.js"></script>
<script src="src/score.js"></script>
```

> **提示**：也可以使用現代 ES Modules（`type="module"` / `import` / `export`），但請搭配本機伺服器（如 VS Code Live Server）測試以避免瀏覽器 CORS 限制。
