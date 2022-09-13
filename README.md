# tataru-helper-node-text-v2

此為 Tataru Helper Node v2.0.0 的翻譯對照表，適用於 v2.0.0 或以上版本

## 文件格式

### chs

存放簡體中文校正用文件

-   overwrite: 存放整句轉換的文件，只要檔名不是 hidden.json 皆會被讀取，格式為[日文, 簡體中文]
-   afterTranslation.json: 存放翻譯後的校正詞彙，格式為[翻譯後欲修正的詞彙, 修正後的詞彙]
-   chName.json: 存放用於建立臨時 NPC 名字的文件，格式為[日文, 簡體中文]

### cht

存放繁體中文校正用文件

-   overwrite: 存放整句轉換的文件，只要檔名不是 hidden.json 皆會被讀取，格式為[日文, 繁體中文]
-   afterTranslation.json: 存放翻譯後的校正詞彙，格式為[翻譯後欲修正的詞彙, 修正後的詞彙]
-   chName.json: 存放用於建立臨時 NPC 名字的文件，格式為[日文, 繁體中文]

### en

存放英文校正用文件

-   ignore.json: 存放例外句子的文件，開啟「忽略常見系統訊息」時在此文件內的句子皆會被略過不翻譯，格式為[英文(正規表達式)]

### jp

-   subtitle: 存放片段日文句子的文件，用於更改原文句子使之更容易被翻譯引擎正確地翻譯，只要檔名不是 hidden.json 皆會被讀取，替換順序為 subtitle>jp1>jp2，格式為[日文, 日文]
-   ignore.json: 存放例外句子的文件，開啟「忽略常見系統訊息」時在此文件內的句子皆會被略過不翻譯，格式為[日文(正規表達式)]
-   jp1.json: 存放日文片段的文件，用於更改原文句子使之更容易被翻譯引擎正確地翻譯，替換順序為 subtitle>jp1>jp2，格式為[日文, 日文]
-   jp2.json: 存放日文片段的文件，用於更改原文句子使之更容易被翻譯引擎正確地翻譯，替換順序為 subtitle>jp1>jp2，格式為[日文, 日文]
-   kana.json: 存放平假名和片假名的文件，格式為[平假名, 片假名]
-   listCrystalium.json: 存放部分第一世界 NPC 名字的文件，在 5.0 台詞「公」大多是指水晶公，但翻譯引擎並不會如此辨認，故建立此文件來修正，只要是在這名單內的 NPC 講的公都會被翻譯成水晶公，格式為[日文]
-   listHira.json: 存放需要將台詞轉換成片假名的 NPC 名單，格式為[日文]

### main

存放詞彙校正用文件，也是最主要的替換文件，所有 NPC 名字和專有名詞皆使用此文件進行替換，只要檔名不是 hidden.json 皆會被讀取，N/A 代表尚待補充，在讀取時會被自動刪除，格式為[日文, 英文, 繁體中文, 簡體中文]

### readme

Tataru Helper Node 使用說明書

### remain

待整理區

## 翻譯錯誤回報方式

### 使用 Tataru Helper Node 回報

1. 在 Tataru Helper Node 視窗點選欲回報的字幕，然後點選【回報翻譯錯誤】按鈕

### GitHub 簡易回報

1. 申請 GitHub 帳號，已有帳號的人直接看第 2 步驟
2. 按下左上角的「Issues」，再按下右上角的「New issue」(綠色按鈕)，填寫需要修正的詞彙之後按下「Submit new issue」即可

### GitHub 詳細回報

1. 申請 GitHub 帳號，已有帳號的人直接看第 2 步驟
2. 按下本專案右上角的「Code」按鈕(綠色按鈕)，然後按「Download ZIP」即可下載整個專案文件
3. 下載後開啟文字編輯器來編輯對照表，請依照下方格式來修改，.json 檔可以用記事本開啟，但建議使用 Notepad++進行編輯的動作
4. 回到https://github.com/winw1010/tataru-helper-node-text-ver.2.0.0 ，登入 Github 帳號後按下右上角的「Fork」將本專案複製到你的帳號裡
5. 將稍早修改的對照表拖曳上傳到上一步驟 fork 下來的專案並完成 Commit 的動作，然後按下「New pull request」按鈕，再按下「Create pull request」按鈕就能送出修改請求

## 特別感謝

簡體中文翻譯: 夜北 yakita
