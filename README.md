# 🏁 Pitstop (<1824>-pitstop)

> 這是我們團隊的第一個協作專案！  
> 本專案為高中「遊戲製作人」課程第 6 課的分組協作作業。

---

## 📖 專案簡介

本專案採用極簡 **HTML5 Canvas** 與 **原生 JavaScript (Vanilla JS)** 開發，打造經典的直向街機風格遊戲原型。

- **畫布規格**：寬度 480px × 高度 640px（直向 Arcade 比例）。
- **當前功能**：
  - 玩家角色為綠色方塊，置於畫面底部中央。
  - 支援使用鍵盤「左/右方向鍵（`←` / `→`）」或「`A` / `D`」控制左右移動。
  - 具備左右邊界碰撞檢查，避免玩家方塊移出畫布。
  - 主遊戲循環（Game Loop）採用 `requestAnimationFrame`，提供流暢畫面更新。

---

## 📂 專案檔案結構

```text
1824-pitstop/
├── index.html        # 遊戲主頁面、畫布設定與主循環邏輯
├── src/              # 模組預留目錄（供組員擴充各自分工功能）
│   ├── README.md     # 模組引入說明與分工建議
│   └── player.js     # 玩家模組範本
├── .gitignore        # Git 忽略清單
└── README.md         # 專案說明文件（本檔案）
```

---

## 🚀 快速開始 (Quick Start)

### 方式一：直接開啟
直接以任何現代網頁瀏覽器（Chrome、Edge、Firefox、Safari）按兩下開啟 `index.html` 即可立即遊玩與測試。

### 方式二：使用 Live Server（推薦）
若組員使用 VS Code，可安裝延伸模組 **Live Server**，在 `index.html` 上按右鍵選擇 **「Open with Live Server」**，即可在儲存檔案時自動即時預覽更新。

---

## 🎮 操作說明

| 操作按鍵 | 動作 |
| :--- | :--- |
| <kbd>←</kbd> 或 <kbd>A</kbd> | 方塊向左移動 |
| <kbd>→</kbd> 或 <kbd>D</kbd> | 方塊向右移動 |

---

## 👥 團隊協作與分工指南

為了讓組員協作順利且避免 Git 衝突（Conflict），建議遵守以下協作原則：

1. **模組化分工**：
   - 請將新功能（如計分板、道路障礙物、音效管理等）獨立撰寫於 `src/` 目錄下的專屬 `.js` 檔案中。
2. **分支開發流程 (Branching Strategy)**：
   - 避免直接推送到 `main` 分支。
   - 每次開發新功能請從最新 `main` 建立獨立分支：
     ```bash
     git checkout -b feature/obstacles  # 障礙物功能分支範例
     ```
   - 完成並測試後提交 Pull Request (PR) 進行合併。
3. **提交訊息規範 (Commit Message)**：
   - 保持 Commit 簡潔清晰，例如：
     - `feat: 加入障礙物下落與碰撞判定`
     - `style: 優化遊戲畫布陰影與跑道背景`
     - `fix: 修復玩家方塊右邊界穿透問題`

---

## 🛠️ 開發環境與技術棧

- HTML5 / CSS3
- HTML5 Canvas API
- JavaScript (ES6+)
- Git & GitHub
