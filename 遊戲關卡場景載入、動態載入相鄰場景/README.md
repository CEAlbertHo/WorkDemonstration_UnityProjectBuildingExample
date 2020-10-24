# 遊戲關卡場景載入、動態載入相鄰場景

## -簡介-
載入遊戲的初始場景，並在符合觸發條件時，額外載入指定場景。
![Load New Game](https://i.ibb.co/FJ3rVdg/Load-New-Game.gif)


依照目前的撰寫設計，載入指定關卡的時候，會同時載入這個關卡相連 ( 可以透過傳送門走過去 ) 的關卡。
所以新遊戲點下去的時候，會先載入 "Stage_00001" ( 指定目標關卡 )，接著查表載入 "Stage_00002" ( Stage_00001 的相鄰關卡 )。

![Process Enter Stage](https://i.ibb.co/xjr1LvM/Process-Enter-Stage.png)

![Check And Load Connecting Stage](https://i.ibb.co/KNrHj42/Check-And-Load-Connecting-Stage.png)

目前的設計是當玩家碰觸到掛載腳本的物件 ( 掛載自己寫的 Component & Collider2D 元件 ) ，並且類行為傳送門類型時，查表查出傳送目標關卡及位置，並且會重複上面提到的 CheckAndLoadConnectingStage 來預先載入相鄰的關卡 ( 以目前的範例來說，Stage_00002 會和 Stage_00003, Stage_00004 相連 )。
![Dynamic Load Stage _ 40percent](https://i.ibb.co/vcMZbXs/Dynamic-Load-Stage-40percent.gif)
( 補充 : 因為 GIF 原圖太大，所以有做縮小處理. 原圖位置 )