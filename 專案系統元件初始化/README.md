# 專案系統元件初始化

## -簡介-
系統元件的啟動途徑。

在 [專案啟動程序](https://github.com/CEAlbertHo/WorkDemonstration_UnityProjectBuildingExample/tree/master/%E5%B0%88%E6%A1%88%E5%95%9F%E5%8B%95%E7%A8%8B%E5%BA%8F) 跑完之後，主要的場景會被切換成 Core 場景。

Core 物件上面的 Component 裡面有初始化的方法，而這個方法會在確認場景載入完畢後被呼叫。
![Core Obj Component](https://i.ibb.co/gTvxwfr/Core-Obj-Component.png)

被呼叫的方法會再去呼叫各個系統的初始化方法。
![Core Obj InitSystem](https://i.ibb.co/4M5jYHT/Core-Obj-Init-System.png)