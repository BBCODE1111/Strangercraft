# Strangercraft 怪奇麥塊物語

走進 Hawkins，和朋友一起找回失蹤的 Will，穿越顛倒世界，迎接現實學校裡的決戰。

**Strangercraft** 是以《怪奇物語》第一季為靈感的 Minecraft Java 合作冒險，支援 **1–6 人**。你可以獨自遊玩，也可以與朋友分工探索、救援與牽制魔神。

這是一個單純的《怪奇物語》粉絲作品，簡化並改編了許多劇情流程，沒有追求高度還原。製作它的初衷，只是希望帶來沉浸的體驗，讓你感受走進顛倒世界的氣氛。

目前下載版本：**V6.4.7｜黎明的代價**。

## 下載

| 你要做什麼 | 下載哪一包 |
| --- | --- |
| 第一次玩，或準備當房主 | [完整遊戲包：Strangercraft-v6.4.7.zip](https://github.com/BBCODE1111/Strangercraft/releases/download/v6.4.7/Strangercraft-v6.4.7.zip) |
| 只加入朋友的房間 | [朋友端：Strangercraft-v6.4.7-players.zip](https://github.com/BBCODE1111/Strangercraft/releases/download/v6.4.7/Strangercraft-v6.4.7-players.zip) |
| 已有 Fabric 與 Fabric API，只補遊戲模組 | [Hawkins V6.4.7 模組](https://github.com/BBCODE1111/Strangercraft/releases/download/v6.4.7/hawkins-escape-6.4.7.jar) |

[查看所有下載檔案](https://github.com/BBCODE1111/Strangercraft/releases/tag/v6.4.7)

完整遊戲包包含兩個必要模組、乾淨世界、獨立伺服器、Fabric 安裝器與遊玩說明。朋友端包含兩個必要模組、Fabric 安裝器與說明；加入朋友時不需要自己裝世界。

請下載上表的遊戲包。GitHub 自動提供的 **Source code** 壓縮檔只有這個專案的介紹與說明，無法直接遊玩。

## 你會玩到什麼

- **Hawkins 探索**：從地下室的 D&D 聚會出發，追查 Byers 家的供電，深入森林救出 Will。
- **顛倒世界**：被木質根系侵蝕的街道、房屋與學校，紅色天空、雷光與飄落的灰燼。
- **聲音與潛行**：魔神會聽見走路、奔跑和道具聲響，也會在正面看見你。利用轉角、家具與窄通道躲避，蹲下減少腳步聲。
- **合作救援**：隊友倒地後有 60 秒救援時間；逾時會被囚禁在森林，仍能等同伴營救。
- **道具牽制**：空罐、煙火、水槍、樂器與火把，各有吸引注意或爭取時間的用途。
- **學校決戰**：全隊一起返回現實，掩護 Eleven 充能與施法。她倒下時只重試決戰。
- **對講機任務提示**：右鍵查看目前目標，以大字閱讀框呈現；R 收起，長訊息可翻頁。

[閱讀完整遊戲說明](docs/GAMEPLAY.md)

## 遊戲需求

| 項目 | 使用版本 |
| --- | --- |
| Minecraft | **Java Edition 1.21.1** |
| Fabric Loader | **0.16.14** |
| Fabric API | **0.116.17+1.21.1** |
| Hawkins 模組 | **6.4.7** |
| Java | **21** |
| 人數 | **1–6 人** |

所有玩家和伺服器使用同樣的模組版本。每個人的 `mods` 只需要這兩個檔案：

```text
fabric-api-0.116.17+1.21.1.jar
hawkins-escape-6.4.7.jar
```

Minecraft Bedrock／手機／主機版不能加入這個 Java Fabric 遊戲。

## 安裝與開局

1. 安裝 Minecraft Java 1.21.1 和 Fabric Loader 0.16.14。
2. 建立獨立的遊戲目錄，把遊戲包內的兩個模組放入 `mods`。
3. 房主把乾淨世界放入 `saves`，朋友只需加入房間。
4. 同一區網由房主按 Esc →「開放至區域網路」；不同網路使用獨立 Fabric 伺服器。
5. 大家到齊後，房主輸入 `/hawkins start`。

[逐步安裝說明](docs/INSTALL.md) · [跨網與獨立伺服器開局](docs/SERVER.md)

美術與音效已內建在遊戲模組，正常遊玩不用另外啟用資源包或安裝光影。

## 官方安裝工具

- [Minecraft 官方啟動器](https://www.minecraft.net/download)
- [Fabric 官方安裝器](https://fabricmc.net/use/installer/)：安裝時選 **Minecraft 1.21.1／Loader 0.16.14**。
- [Java 21（Eclipse Temurin）](https://adoptium.net/temurin/releases/?version=21)：選符合自己電腦的作業系統與架構。

Strangercraft 是玩家創作的冒險模組，並非 Minecraft 或《怪奇物語》的官方作品。
