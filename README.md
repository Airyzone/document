# AIRYZONE IoT 解決方案

![](https://github.com/Airyzone/document/raw/master/resource/image/iot_service.png)
* 基本組件
    * AIRYZONE Beacon（移動信標)
        * 基於低功耗藍牙的硬體裝置，不斷廣播藍牙訊號，夾帶唯一性內碼資訊。
        * 依照應用情境的私密性與複雜度，廣播資訊可以設定為靜態或動態、加密或公開。
        * 可以依照各種應用情境需求添加各種感知器，例如溫度計、3軸加速度計、紫外線照度計......等。
        * 輕薄短小，可以多樣化的形式存在，例如：手環、寵物項圈、名片......等。
        * 省電，在基本功能之下，使用一顆CR3202電池大約可以維持半年至一年的操作。
        * 除了AIRYZONE自行開發販售之AIRYZONE Beacon之外，尚提供AIRYZONE Beacon SDK供參與合作的開發者自行設計硬體與韌體，嵌入AIRYZONE Beacon SDK的韌體即能擁有AIRYZONE Beacon的核心功能。
    * AIRYZONE Beacon SDK（移動信標韌體開發套件）
        * 參與合作計畫的開發者可以嵌入引用此套件開發自有韌體，即能擁有AIRYZONE Beacon之核心功能。
        * 目前提供Nordic Semiconductor nRF52832藍牙單芯片之開發套件，基於ARM Keil MDK開發環境（使用C語言）。
    * AIRYZONE Detector（偵測器）
        * 基於低功耗藍牙的硬體裝置，不斷掃描接收由AIRYZONE Beacon發出的廣播訊號，解析移動標籤資訊之後，經由Ethernet、Wi-Fi或電信網路傳送資訊到AIRYZONE Cloud。
        * 除了以專用硬體的形式存在之外，任何智慧型手機（iOS、Android系統）安裝了嵌入AIRYZONE Detector SDK的手機應用程式（APP），皆可以擔任Airyzone Detector的角色功能。
    * AIRYZONE Detector SDK（偵測器手機應用程式開發套件）
        * 目前提供iOS與Android手機作業系統的應用程式開發者套件。
        * 提供Swift語言（iOS）與Java語言（Android）的原生函示庫套件、API說明與應用程式範例。
        * 參與合作計畫的開發者可以在熟悉的語言開發環境內嵌入函示庫，透過呼叫API，自行開發應用程式，此應用程式即能擔任AIRYZONE Detector的角色，並擁有存取AIRYZONE IoT Service相關功能。
    * AIRYZONE Cloud（雲）
        * 網路雲端設備，用於AIRYZONE IoT Service相關應用。
![](https://github.com/Airyzone/document/raw/master/resource/image/cloud.png)
    * AIRYZONE IoT Service（物聯網服務）
        * 由多個Beacon、多個Detector與Cloud組成之生態鍊。可以將各個Beacon節點的資訊連結，經過雲端計算之後，達成特定目的的服務。
        * 目前主要的服務包含：定位、資料收集與協尋三大類，並衍伸出各式變形。
