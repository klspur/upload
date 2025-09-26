# 酒精大富翁（ALCO_monopoly.html）

## 如何把專案放到 GitHub 並測試
1. **在本機建立 Git 儲存庫**
   ```bash
   git init
   git add ALCO_monopoly.html
   git commit -m "Initial commit"
   ```
2. **在 GitHub 建立新的 Repository**（例如 `alcohol-monopoly`），不要勾選自動建立 README。
3. **把遠端加到本機並推送**
   ```bash
   git remote add origin https://github.com/<你的帳號>/alcohol-monopoly.git
   git push -u origin main
   ```
   > 如果你的預設分支是 `master`，請把命令裡的 `main` 換成 `master`。
4. **啟用 GitHub Pages**：進入該 repository 的 **Settings → Pages**，在 "Branch" 選擇 `main`（或 `master`）與 `/root`，儲存後等待幾分鐘，GitHub 會提供一個 Pages 網址，例如 `https://<你的帳號>.github.io/alcohol-monopoly/`。
5. **測試主機介面**：在桌機或筆電瀏覽器打開 `https://<你的帳號>.github.io/alcohol-monopoly/ALCO_monopoly.html`，即可看到主控台畫面。
6. **讓手機加入**：主機畫面會顯示 QR Code，使用手機掃描後就能打開 `?join=<房間代碼>` 的連結；輸入暱稱上傳大頭貼即可加入。

> 若要同步更新 GitHub 上的檔案，只需要在本機修改後 `git add` + `git commit` + `git push` 即可。GitHub Pages 會在推送後自動重新部署。

## 行動裝置操作重點
- 每位手機玩家都可以在自己的裝置上查看目前輪到誰、骰子點數、玩家列表與最新事件。
- 當停在格子或抽卡時，手機會同步顯示翻卡畫面，並由當回合的玩家負責按下「翻開內容」與「了解，執行」。
- 若連線中斷，可重新掃描 QR Code 再次加入，同一支手機會沿用先前的大頭貼與暱稱。

## 推薦測試方式
1. 主機端以桌機開啟 GitHub Pages 的主控畫面。
2. 以 2 支以上手機掃描 QR Code 加入遊戲。
3. 測試以下情境：
   - 手機上傳大頭貼與暱稱。
   - 手機擲骰、結束回合。
   - 手機翻開停格內容及抽卡，確認桌機同步顯示。
   - 斷線重連後是否能重新加入。

祝遊戲順利，請理性飲酒！
