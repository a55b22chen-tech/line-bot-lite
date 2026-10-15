# LINE bot 輕量版（W6 回家作業）

這是老師提供的 Python 範例，使用電腦上的 Ollama 小模型回答文字問題。先做必做的模擬模式，不接 LINE。

## 怎麼安裝

1. 安裝 Python 3 和 Ollama。
2. 開啟 PowerShell，下載模型：`ollama pull gemma4:e2b`。
3. 模型下載完成後，開啟放有 `line_bot_lite.py` 的資料夾；在檔案總管的網址列輸入 `powershell`，按 Enter，就會在該資料夾開啟 PowerShell。

## 怎麼執行

在 PowerShell 輸入：

```powershell
python line_bot_lite.py --simulate
```

看到 `📱 你：` 後輸入問題，等 Bot 回覆。輸入 `quit` 結束。模擬模式不需要 LINE 通行碼，也不會連接 LINE。

## 我改了什麼

目前使用老師提供的原版程式，沒有修改程式內容。2026-10-15 在本機實際執行模擬：模型為 `gemma4:e2b`；第一次載入 11 秒，問候語立即回覆，玉山問題和最近事件問題各約 2 秒。Ollama 回報 `size_vram: 0`，本次沒有使用顯示卡記憶體；電腦是否有顯示卡尚未確認。測試過程沒有卡住，LINE 串接尚未嘗試（選做）。

## 參考

- [互動指南](https://cwstedctw.github.io/ndhu-ted-course-hub/weekly/11501-ai-coding/w06/line-bot-lite.html)
- [老師提供的原始程式](https://cwstedctw.github.io/ndhu-ted-course-hub/weekly/11501-ai-coding/w06/starter/line_bot_lite.py)
