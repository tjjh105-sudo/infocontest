# ⚾ E起挺 Taiwan：2024 世界棒球 12 強選球特訓遊戲

[cite_start]這是一款專為棒球愛好者設計的 **HTML5 選球訓練遊戲**。透過捕手視角的九宮格好球帶，玩家可以練習判斷多種變化球路 [cite: 6][cite_start]。本遊戲最大的特色在於「單一 HTML 檔案即可執行」，無需任何外部圖檔、音檔或後端資料庫 [cite: 70, 75, 92]。

詳細的開發歷程與設計規格請參考：[**一起挺台灣AI.pdf**](./一起挺台灣AI.pdf)

## 🌟 遊戲特色

* [cite_start]**專業球路模擬** [cite: 6, 12]：
    * [cite_start]**四縫線快速球 (Fastball)**：軌跡最直、速度最快 [cite: 13]。
    * [cite_start]**曲球 (Curveball)**：速度較慢，模擬垂直墜落感 [cite: 14]。
    * [cite_start]**滑球 (Slider)**：中等球速，在路徑後段增加橫向偏移誘使打者出棒 [cite: 15]。
    * [cite_start]**卡特球 (Cutter)**：模擬快速球但在接近本壘板時產生微幅橫向位移 [cite: 16]。
* [cite_start]**熱血視覺與情境** [cite: 31, 32]：
    * [cite_start]**教練登場動畫**：遊戲啟動時由具備兩片式墨鏡的「教練」說明 2024 年世界棒球 12 強賽背景 [cite: 29, 38]。
    * [cite_start]**愛國元素**：教練球帽上設有國旗圖案，且畫面右上方設有飄揚的中華民國國旗 [cite: 99, 100]。
* [cite_start]**技術回饋機制** [cite: 17, 21]：
    * [cite_start]系統會紀錄使用者的「追逐壞球」與「看著好球進壘」比例 [cite: 18]。
    * [cite_start]根據表現給予「增加耐性」或「增加攻擊性」等技術回饋建議 [cite: 19, 20]。

## [cite_start]🛠️ 技術原理：為何能「單檔執行」？ [cite: 79]

1.  [cite_start]**圖像處理 (內嵌 SVG)** [cite: 80]：
    * [cite_start]教練角色直接使用內嵌 SVG 程式碼繪製，無需下載外部圖片 [cite: 47, 83]。
    * [cite_start]可透過 CSS 控制教練呼吸起伏，以及 JavaScript 控制說話時的嘴型動畫 [cite: 59, 67, 82]。
2.  [cite_start]**音訊工程 (Web Audio API)** [cite: 84]：
    * [cite_start]BGM 透過 `AudioEngine` 虛擬合成器即時運算，使用振盪器（OscillatorNode）產生旋律 [cite: 86, 87]。
    * [cite_start]支援雙階段 BGM：引導階段平穩，投球階段自動切換為 145 BPM 的熱血節奏 [cite: 40, 41]。
3.  [cite_start]**語音系統 (Web Speech API)** [cite: 88, 89]：
    * [cite_start]直接呼叫裝置內建的文字轉語音引擎 (TTS Engine)，反應速度達到「零延遲」 [cite: 90, 91]。

## 🎮 操作方式

* [cite_start]**策略**：注意球在最後一刻的變化，球移動具備立體縮放感模擬深度 [cite: 10, 24]。
* [cite_start]**互動**：點擊螢幕下方的「揮棒」或「不揮」進行判斷 [cite: 23]。

---
**讓我們一起在這熱血的氣氛中挺台灣！** 🇹🇼