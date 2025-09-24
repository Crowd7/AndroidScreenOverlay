Android app to generate a overlay screen for testing tapjacking protection

🔹 測試方式

1. 安裝並跑這個 App。

2. 點擊畫面中按鈕

3. 首次執行會跳出「允許在其他應用程式上層顯示」 → 打開。

4. 畫面會出現紅色半透明遮罩。

5. 這時候去點擊你自己要測試的 Activity → dispatchTouchEvent 裡應該會抓到 ev.flags 被標記。

官方文件：
https://developer.android.com/privacy-and-security/risks/tapjacking?hl=zh-tw
