# 安裝 Strangercraft

## 1. 下載遊戲包

- 第一次玩或當房主：[完整遊戲包](https://github.com/BBCODE1111/Strangercraft/releases/download/v6.4.11/v6.4.11.zip)。
- 只加入朋友：使用同一個完整包裡的 `玩家端/mods`，不需複製房主世界。

解壓縮後再使用。所有人固定使用 Minecraft Java **1.21.1**、Fabric Loader **0.16.14** 和 Hawkins **6.4.11**。

## 2. 準備 Minecraft 與 Java

1. 安裝 [Minecraft 官方啟動器](https://www.minecraft.net/download)，登入自己的正版帳號。
2. 在「安裝檔」建立 **Java 1.21.1**，先啟動一次，再退出並關閉遊戲與啟動器。
3. 執行 Fabric 安裝器或獨立伺服器需要可用的 Java。若沒有，從 [Java 21 官方下載](https://adoptium.net/temurin/releases/?version=21) 安裝。

| 電腦 | Java 下載選擇 |
| --- | --- |
| 一般 Intel／AMD Windows | Windows / x64 / JDK / MSI |
| Apple 晶片 Mac | macOS / aarch64 / JDK / PKG |
| Intel Mac | macOS / x64 / JDK / PKG |
| 其他電腦 | 選對應的作業系統和架構 |

Mac 可在「關於這台 Mac」確認晶片種類。Windows Java 安裝時啟用加入 PATH。每台只安裝符合自己的那一份。

## 3. 安裝 Fabric

使用遊戲包 `安裝工具/Fabric/fabric-installer-1.1.2.jar`，或從 [Fabric 官方網站](https://fabricmc.net/use/installer/) 下載安裝器。

開啟安裝器並選：

- **Client**
- Minecraft Version：**1.21.1**
- Loader Version：**0.16.14**
- 安裝到官方啟動器實際使用的 Minecraft 目錄，建立啟動選項。

安裝器 **1.1.2** 是工具版本；你要選的 **Loader** 版本是 **0.16.14**。

若無法直接開啟 `.jar`，在安裝器所在資料夾開終端機執行：

```sh
java -jar fabric-installer-1.1.2.jar
```

## 4. 建立獨立遊戲目錄

在 Minecraft 啟動器「安裝檔」新增遊玩選項：

- 名稱建議：`Strangercraft V6.4.11`
- 版本：`fabric-loader-0.16.14-1.21.1`
- 遊戲目錄：指定一個新的空資料夾，例如文件裡的 `Strangercraft_V6.4.11`。

將遊戲包 `玩家端/mods` 複製到這個新目錄。完成後應該是：

```text
Strangercraft_V6.4.11/
└── mods/
    ├── fabric-api-0.116.17+1.21.1.jar
    └── hawkins-escape-6.4.11.jar
```

不要將其他 Hawkins 版本放進同一個 `mods`。Fabric 安裝器、Java 安裝檔與伺服器啟動檔也不放在 `mods`。

## 5. 房主裝世界

只有房主需要這一步；朋友直接加入即可。

關閉 Minecraft，把完整遊戲包中 `房主世界/saves/Hawkins_Escape_v6_4_11` 複製到新遊戲目錄的 `saves`：

```text
Strangercraft_V6.4.11/
├── mods/
└── saves/
    └── Hawkins_Escape_v6_4_11/
        ├── level.dat
        ├── hawkins_escape.json
        ├── region/
        └── datapacks/
```

若目標已有同名世界，先把新副本改名，例如 `Hawkins_Escape_v6_4_11_多人新局_01`，再複製。不要覆蓋原世界。

啟動剛建立的 Fabric 選項，單人遊戲選 **HAWKINS｜Secret Castle · V6.4.11（無光影）**。若清單有兩個同名世界，以清單顯示的存檔資料夾名稱辨認新副本。

## 6. 朋友加入

### 同一個 Wi-Fi／區網

1. 房主進世界，Esc →「開放至區域網路」，遊戲模式選冒險。
2. 朋友在「多人遊戲」選房間；找不到時用「直接連線」，輸入 `房主區網IP:畫面顯示的埠`。
3. 最多六人；所有人到齊後房主輸入 `/hawkins start`。

每次重開区網時埠可能改變，以當次畫面為準。房主退出世界後朋友會斷線，進度存在房主的世界。

### 不同網路

請看 [獨立伺服器與跨網連線](SERVER.md)。每位玩家仍要安裝相同的兩個模組。

## 資源與音效

美術、自製音效與原版音樂引用已包含在 Hawkins 模組內，不必另外啟用資源包。完整包的 `資源包備份` 只供備份使用。

## 常見問題

- **找不到 Fabric 啟動選項**：在啟動器「安裝檔」啟用顯示已修改版本，確認 Fabric 安裝到啟動器使用的目錄。
- **提示版本不相容**：確認 Minecraft 1.21.1、Loader 0.16.14，以及兩個正確的 jar。
- **同時出現多個 Hawkins**：建立全新遊戲目錄，再放入本包兩個模組。
- **連不到朋友**：同區網使用區網 IP；不同網路使用房主提供的可連入伺服器地址。
- **想重玩但保留舊進度**：從完整包再另存一個乾淨世界，不要覆蓋原世界。

[返回介紹](../README.md) · [遊戲說明](GAMEPLAY.md)

## 更新既有進度

請按完整包內 `更新既有進度.txt`，另存遊戲目錄與世界副本，再替換副本模組。V6.4.7／V6.4.8 還需更新指定資料包 JSON；V6.4.9／V6.4.10 不需要。停用舊 Hawkins 資源包，讓新版地圖生效。舊世界與啟動選項保留，首次載入自動升級場景，不需 restart。

## 玩家 Skin 與音樂

Java 1.21.1 支援自己的 Skin；登入個人帳號，在官方啟動器 Java Edition → Skins 設定。模組沒有替換玩家造型。

戶外沿用原版音樂，間隔約 15–30 秒。請開啟「音樂」音量，與「音效」音量分開。
