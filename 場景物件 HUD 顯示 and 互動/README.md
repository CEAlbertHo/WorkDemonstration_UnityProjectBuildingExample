# 場景物件 HUD 顯示 and 互動

## -簡介-
當玩家進到互動範圍 ( 透過 OnTriggerEnter2D 觸發 ) 的時候，會去通知並設定 HUD 這個 UI 來顯示互動按鈕。

![HUD OnOff Display Demo](https://i.ibb.co/LS8Mq9L/HUD-On-Off-Display-Demo.gif)
( Github 往只有掛掉的話，[備用連結](https://i.ibb.co/LS8Mq9L/HUD-On-Off-Display-Demo.gif) )


玩家點下互動按鈕的時候，會根據互動類型，來執行對應的效果處理。
![HUD HP Interact Demo](https://i.ibb.co/3kzJ02P/HUD-HP-Interact-Demo.gif)