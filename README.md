# Puppy and Annoying Fly — Rive Web Demo

可直接部署到 GitHub Pages 的最小 Rive Web 範例。

## 檔案設定

- Rive file: `puppy_and_annoying_fly.riv`
- Artboard: `Doggie follow`
- State machine: `State Machine 1`

`index.html` 使用官方 Rive Canvas Web runtime。State Machine 會自動播放；Rive Listener 會接收 Pointer Move、Pointer Down、Pointer Up 與 Drag。觸控拖曳時停用頁面捲動，避免手勢被瀏覽器攔截。

## 本機預覽

請勿直接雙擊 `index.html`，因為瀏覽器通常會阻擋本機網頁讀取 `.riv`。

在此資料夾啟動任一靜態檔案伺服器，再開啟它提供的網址。例如使用 Python：

```sh
python3 -m http.server 8000
```

接著開啟 <http://localhost:8000/>。

## GitHub Pages

1. 在 GitHub 建立一個 public repository。
2. 將此資料夾內全部檔案上傳到 repository 根目錄。
3. 開啟 **Settings → Pages**。
4. 在 **Build and deployment** 選 **Deploy from a branch**。
5. 選擇 **main**、**/(root)**，再按 **Save**。
6. 等候 GitHub 顯示網站網址，通常格式為 `https://你的帳號.github.io/repository名稱/`。

若日後在 Rive 重新命名 artboard 或 state machine，只要修改 `index.html` 上方的 `ARTBOARD` 與 `STATE_MACHINE` 常數。
