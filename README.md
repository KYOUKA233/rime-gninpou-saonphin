# 寧波話雙拼輸入方案

配方：℞ **ionkaon/rime-gninpou-saonphin**

本倉庫依賴 [寧波話吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_gninpou)。

寧波話雙拼輸入方案。含老派、新派兩個方案。不設模糊音，故要求使用者已熟練掌握寧波話字音。

- 老派：`gninpou_saonphin.schema.yaml`
- 新派：`gninpou_saonphin_shinpha.schema.yaml`

方案不區分清濁鼻邊音。

不分清濁鼻邊音的話，寧波話有 29 個聲母，考慮到 n、gn 兩個聲母無對立，可以合併爲 28 個。老派有 49 個韻母，新派有 39 個韻母，均大於拉丁字母個數 26。不計鼻音、邊音聲母的清濁對立，也不計聲調，老派寧波話有 551 個不同的音節，新派則有 498 個音節。分別佔雙拼編碼空間（26² = 676）的 81.51 % 和 73.67 %。因此要同時對聲母、韻母做歸併，纔能塞進編碼空間。聲母中，c 組齊齒呼歸入了 ts 組，撮口呼則放到 p 組的位置；ts 組接 -yun、-yuq 韻母時，放到了 t 組的位置；i、y、w 獨立爲單獨的聲母。韻母歸併較多較雜，不詳述，具體可以看表格。

老派的音節表如下：

![音節表（老派）](./assets/音節表（老派）.png)

音節表中紅色是飛鍵，需要單獨記憶。

新派可以少很多飛鍵，僅需記憶 er、m、n、ng、kiq 這五個音節。

![音節表（新派）](./assets/音節表（新派）.png)

按鍵鍵位如下。

老派：

![按鍵（老派）](./assets/按鍵（老派）.png)

新派（刪除了新派沒有的韻母，ioq 韻挪了位置）：

![按鍵（新派）](./assets/按鍵（新派）.png)

鍵位一定程度上參考了自然碼雙拼。未針對寧波話做優化，手感不一定好。

安裝及使用請參考 [寧波話吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_gninpou)。安裝前需先安裝 [寧波話吳語拼音輸入方案](https://github.com/NGLI/rime-wugniu_gninpou)。

## 聯繫

[Shin Zoqchiuq](https://github.com/shinzoqchiuq)：

- 郵箱：shinzoqchiuq@outlook.com
- QQ：1613023143
