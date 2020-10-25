# UI 實作範例

## -簡介-
這邊是接續 [場景物件 HUD 顯示 and 互動](https://github.com/CEAlbertHo/WorkDemonstration_UnityProjectBuildingExample/tree/master/%E5%A0%B4%E6%99%AF%E7%89%A9%E4%BB%B6%20HUD%20%E9%A1%AF%E7%A4%BA%20and%20%E4%BA%92%E5%8B%95) 的部分。
目前的互動類型設定為一般互動的時候，會開啟對話視窗 UI。

![UI Interact Demo](https://i.ibb.co/Jkqgzmn/UI-Interact-Demo.gif)
UI 的部分是很一般的點擊事件，比較特別的是為了處理對話，所以另外寫了一個 DialogueManager，特別用來處理對話以及對話演出 ( 預定之後要新增 ) 的部分。
