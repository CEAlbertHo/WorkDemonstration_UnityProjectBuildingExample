# 按鍵輸入操作 and  設定

## -簡介-
透過 Input Manager 來實現按鍵對應的動作。
由於 Unity 新推的 Input System 在實作這個功能的時候版本還在 1.0.0，所以先用 Input Manager 來實現。

基本的思路是不打算去在 Input Manager 把按鍵給綁死，所以會在每一幀的 Update 處理下列的事情：
 1. 清除舊的輸入記錄。
 2. 掃描所有要掃描的按鍵並記錄其狀態 ( Input.GetKeyDown、Input.GetKey、Input.GetKeyUp )。

![Input Manager Init](https://i.ibb.co/rsfqRdV/Input-Manager-Init.png)

![Input Mapping Constructor](https://i.ibb.co/HpbYz8B/Input-Mapping-Constructor.png)

然後在每一次的 FixedUpdate 把記錄下來的指令送給玩家輸入處理器來做執行。
目前對應的動作主要是在 Input Mapping Constructor 的時候設定的，預計是在設定值得存檔讀檔功能實作之後，能改成讀出存檔中的設定值，達到玩家能夠設定按鍵對應功能的實作。