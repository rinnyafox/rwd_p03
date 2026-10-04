# RWD_P03｜Penana 重新設計

課程：互動前端與體驗設計（115-1）｜作者代碼：P03

重新設計對象：[Penana](https://www.penana.com)（線上小說閱讀平台）。
這個 repository 放 AI 協作交接紀錄與 Pitch；所有設計證據都在 Figma。

## 連結

- Figma（唯一繳交入口）：<https://www.figma.com/design/3Rv4YWeVh0zaRWVP6HSP3i/RWD_P03_Penana重新設計>
  * 📋 評分總覽：<https://www.figma.com/design/3Rv4YWeVh0zaRWVP6HSP3i/RWD_P03_Penana重新設計?node-id=1-2>
- 交接紀錄：[HANDOFF.md](HANDOFF.md)
- Pitch 與逐字稿：[PITCH.md](PITCH.md)（錄影連結尚未建立）
- 主要 AI 討論串：<https://claude.ai/share/08fbaed9-fdbf-49a5-9a5f-d4e727e6ca82>

## 這次重新設計在做什麼

| 原產品的問題 | 設計主張 |
|---|---|
| 長章節一次拉到底，沒有段落錨點，離開後找不回位置 | 章節內分段導覽＋續讀書籤，並把書籤面板升級為獨立的「閱讀進度」頁 |
| 首頁「小說推薦」卡片版型不一致，無封面作品是灰底純文字 | 書籍卡片改為統一的 Auto Layout 元件，封面為固定插槽 |
| 手機版故事頁的作者、訂閱、催更資訊被擠到頁面下方 | 手機版把贊助、催更、作者資訊上移到主視覺下方 |

裝置寬度：手機 390、桌機 1440（不做平板）。5 個核心畫面：閱讀頁、首頁、故事詳情頁、閱讀進度頁、搜尋結果頁。

## 版本紀錄

| 版本 | 日期 | 在哪裡看 | 重點 | 依據 |
|---|---|---|---|---|
| v1 | 2026-09-27 | Figma 🗄 v1 封存頁；GitHub tag `v1` | 初稿：閱讀頁與故事頁（手機、桌機） | 第一版，依原產品診斷與設計主張初稿 |
| v2 | 2026-10-04 | Figma 🗄 v2 封存頁；GitHub tag `v2` | 主色改為 #9E5C00 修正按鈕對比；補齊 Brief；5 個核心畫面×手機／桌機，含空狀態與錯誤狀態；Button 新增 Focus 變體；通過 320px 重排 | AI 輔助檢核（2026-10-04），記錄於 [HANDOFF.md](HANDOFF.md) |

## 這一版還沒做到的事

- 沒有平板（768）寬度。
- 尚未進行使用者任務測試，Brief 裡的成功指標只是目標，不是結果。
- WCAG 的焦點可見只做到設計層（Button 有 Focus 變體），原型內的焦點順序尚未實測。
- 加分題目前只有一種檢查來源，尚未做第二種工具的交叉檢查。

## 資料安全

此 repository 不包含 API 金鑰、密碼或個人資料；`.gitignore` 已排除 `.env`。
