# 專案啟動程序

## -簡介-
Unity 點下 Play 之後的專案啟動機制。

![Unity Game Start Record GIF](https://i.ibb.co/pQ5W2YQ/Unity-Game-Start-Record-GIF.gif)


透過掛載在原始場景物件上的腳本，使其在啟動 ( Start ) 時先去呼叫 Addressables 做初始化。
![專案 Init Load Scene](https://i.ibb.co/DLJmCqV/Init-Load-Scene.png)

![專案場景 Addressable Group](https://i.ibb.co/cD2PJKR/Addressable-Group.png)

初始化完成後透過自己寫的 AssetsLoader 做異步載入 Addressables 場景資源，接著在 IEnumerator CheckLoadSceneAsync 檢查是否場景資源都載入，都載入之後釋放原本的場景 ( InitGame ) 並做後續的元件初始化。