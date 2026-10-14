# 獨立伺服器與跨網連線

同區網可以直接用「開放至區域網路」。朋友不在同一個網路，或希望房主關閉遊戲後房間仍存在時，可使用獨立伺服器。

## 準備

下載 [完整遊戲包](https://github.com/BBCODE1111/Strangercraft/releases/download/v6.4.7/Strangercraft-v6.4.7.zip)，解壓縮後使用 `獨立伺服器` 資料夾。裡面已提供：

- Minecraft 1.21.1／Fabric Loader 0.16.14 的啟動檔。
- 相同的兩個必要模組。
- 乾淨的 `world`，包含場景設定與 datapack。
- `server.properties`、`eula.txt`、Mac 與 Windows 啟動檔。

先安裝 [Java 21](https://adoptium.net/temurin/releases/?version=21)。伺服器使用最多 3GB 記憶體，主機還需留出系統與 Minecraft 客戶端的使用空間。

請在新的資料夾開服，不要覆蓋其他伺服器的世界。

## 開服

1. 自行閱讀並接受 [Minecraft EULA](https://www.minecraft.net/eula) 後，把 `eula.txt` 的 `eula=false` 改成 `eula=true`。
2. Mac 雙擊 `start.command`；Windows 雙擊 `start.bat`。
3. 首次啟動需網路下載 Minecraft 伺服器、Fabric Loader 與相依檔。等待主控台出現 `Done`。
4. 在伺服器主控台輸入 `op 你的Minecraft玩家名`，讓房主取得開始與重玩的權限。朋友不必都設為 OP。
5. 房主從「多人遊戲」加入 `localhost:25565`；同區網朋友使用 `主機區網IP:25565`。
6. 全員到齊後，房主在遊戲輸入 `/hawkins start`。

Mac 如果不能直接執行腳本，可在伺服器資料夾的終端機輸入 `bash start.command`。Windows 找不到 Java 時，確認安裝 Java 21 並加入 PATH，重開終端機再試。

## 不同網路的朋友如何加入

可選擇：

- **Fabric 伺服器服務**：選能執行 Minecraft Java 1.21.1／Fabric 0.16.14、可上傳自訂模組與世界的服務。上傳本包伺服器的 `mods` 與 `world`，依服務的控制台指定此世界。
- **自己的電腦當主機**：設定主機防火牆與路由器的 TCP 25565 轉發，再把可連入的公網地址給朋友。如果網路有電信 CGNAT 或雙層 NAT，單一路由器轉發可能不足。

不同網路不能用房主的區網 IP。預設連線埠是 25565；若自行更改，以實際設定為準。

GitHub 提供的是遊戲檔下載，遊戲房間仍由你的電腦或 Fabric 伺服器運行。

## 玩家端與資源

每位玩家仍需要 [安裝玩家端](INSTALL.md)，固定使用相同的 Minecraft、Fabric Loader 與兩個模組。美術和音效內建在模組中，不需要另設資源包下載網址。

預設最多六人，`online-mode=true`，使用正版帳號。Java Realms 與原版伺服器不能直接執行此 Fabric 模組。

## 停服與續玩

在主控台輸入 `stop`，等伺服器正常退出後再備份整個資料夾。重新啟動會延續這份世界的進度。

不要同時用兩個伺服器程序開啟同一份世界。想保留舊局並換整批朋友時，另存完整包中的乾淨世界。

[返回介紹](../README.md) · [遊戲說明](GAMEPLAY.md)
