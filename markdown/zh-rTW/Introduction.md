# Vespucci 介紹

Vespucci 是一個完整功能的開放街圖編輯器，支援那些桌面系統編輯器所提供的大部分的操作。它在谷歌 Android 2.3 至 6.0 以及各種 AOSP 為主轉化的。已經過成功地測試。提醒一句：行動裝置能力已經追上桌面系統與之匹敵，尤其是較舊的裝置，只有非常有限的可用記憶體，並且往往是相當緩慢的。在使用  Vespucci 和持有時，您應該考慮到與接受，例如，您正在編輯的區域尺寸是一個合理的大小。 

## 第一次使用

在啟動 Vespucci 時為您顯示 "下載其它位置"/"載入區域" 的對話框。如果您有座標顯示並且想要立即下載，您可以選擇合適的選項，和設定想要的下載半徑週圍位置，請不要在緩慢的裝置上選擇大的面積。 

除此之外您可以透過按按鈕解除對話框，並平移與放大位置到想要編輯和下載的資料(見下方："編輯于 Vespucci")。

## 編輯于 Vespucci

根據畫面尺寸和您裝置的新舊，編輯操作可以經由在頂端列的圖示可直接進入，通過下拉選單中頂端列的右側，從底部列(如果存在的話) ，或者透過選單鍵。

### 下載 OSM 資料

選擇任何一個的傳輸圖示！[](../images/menu_transfer.png)或“傳輸”選單項目都可以。這將顯示七個選項：

 * **下載現在的檢視** - 下載在螢幕上可見的區域，並取代所有目前的資料*(需要網路連線)* 
* **增加現在的檢視來下載** 下載在螢幕上可見的區域，並合併目前的資料*(需要網路連線)* 
* **下載其它地方** - 顯示一個表單，允許您輸入座標搜尋一個位置或直接輸入座標，然後下載該區域週圍的地方*(需要網路連線)* 
* **上傳資料到 OSM 伺服器** - 上傳編輯到 OpenStreetMap *(需要網路連線)*
* **自動下載** - 自動的下載目前周圍位置區域 *(需要網路連線)*  *(需要 GPS)*
* **檔案...** - 儲存和載入在裝置的 OSM 檔案資料。
* **備註/錯誤** - 從 QA 工具 (目前的 OSMOSE) 下載 (自動或手動) OSM 備註和"錯誤" *(需要網路連線)*

打開一張地圖的最簡單方法就是縮放和平移到您想要編輯的地方，然後選擇"下載目前的檢視"。您可以在手機上，通過使用手勢、縮放按鈕或音量控制按鈕進行縮放。Vespucci 應會下載在您目前的位置上的區域和中心地圖的資料。不需要進行驗證就能將所需的資料下載到您的裝置。

### 編輯

為了防止無意中的編輯 Vespucci 開始在"鎖定"模式，這種模式，只允許縮放和移動地圖。點擊！[鎖定] (../images/locked.png) 圖示來解鎖螢幕。預設情況下，可選擇節點和道路周圍有橙色區域大致說明要觸碰選擇一個物件。如果您試著選擇一個物件而 Vespucci 判斷所選內容可能表示著多個物件，將呈現一個選擇選單。選定的物件是以黃色高亮顯示。

如果您試著編輯高密度區域時進行放大，這是一個很好的對策。

Vespucci 擁有一個良好的"取消/重做"系統，所以不要害怕在您的裝置嘗試，但是請不要上傳和儲存純測試資料。

#### 選擇/取消選擇

觸碰物件以選擇和高亮顯示，在元件上對同一物件的第二次觸碰則開啟標籤編輯器。在空白區域上觸碰螢幕則會取消選擇。如果您已選擇了一個物件，您需要選擇別的東西，只需觸碰有問題的物件，沒有必要先取消選擇。對物件按兩下將會開始 [多重選擇模式](Multi-Select.md)。

#### 增加新節點/點或是路徑

在您想要的那個節點或開始的道路長按。您將會看到一個黑色的"十字"符號。再次輕觸相同的位置可建立一個新的節點，觸碰位置為容許偏差範圍之外的接觸位置，那將會從原本的地點到目前的位置增加一段道路。 

當您想要增加道路更遠地節點，只需觸碰畫面。若要完成，觸碰最終的節點兩次。如果初始節點位於一條道路上，節點將被自動插入道路。

#### 移動節點或路徑

只有當物件被選中時可以將它們拖曳或移動。如果您在參數中選擇大面積的拖曳區域，您會得到大面積區域周圍的選取節點，使得它更容易到物件的位置。 

#### 改善道路的幾何形狀

如果您放大到足夠遠的程度，在足夠長的道路段中間，您會看到這樣一個小"x"。拖曳“×”，會建立一個在該位置的節點。注意：為了防止意外的建立節點，此操作的觸碰容差是相當小的。

#### 剪下、複製和貼上

您可以複製或剪下選擇的節點和路徑，然後貼上一次或多次到一個新的位置。剪切將保留 OSM ID 和版本。要貼上長按要貼上的位置(您會看到一個十字線標記的位置)。然後從選單中選擇“貼上”。

#### 有效的增加地址

Vespucci 有一個"增加地址標籤"功能，那讓勘察地址更有效率。它是可以選擇的 

* 經長按後：Vespucci 將增加一個節點的位置，並在門牌號碼做出最佳的推測，和增加您最近一直使用該地址的標籤。如果該節點是在建築物外形上，它將會自動增加 **入口 = 是"" 標籤到節點。該標籤編輯器將打開有疑問的物件，並讓您作更進一步任何的變更。
* 在節點/道路選擇模式：Vespucci 將為上述的增加地址標籤，並啟動標籤編輯器。
* 在標籤編輯器。

門牌號碼預測，一般需求要在道路的兩側，至少兩間房屋號碼需要輸入到作業中，更多的號碼存在於資料中越好。

考量使用這種"自動下載"模式。  

#### 增加轉​​彎限制

Vespucci 有個快速的增加轉向限制。注意：如果您為了限制而需要分割一條道路，您須要在開始之前做到這點。

* select a way with a highway tag (turn restrictions can only be added to highways, if you need to do this for other ways, please use the generic "create relation" mode, if there are no possible "via" elements the menu item will also not display)
* select "Add restriction" from the menu
* select the "via" node or way (all possible "via" elements will have the selectable element highlighting)
* select the "to" way (it is possible to double back and set the "to" element to the "from" element, Vespucci will assume that you are adding an no_u_turn restriction)
* set the restriction type in the tag menu
 
### Vespucci in "locked" mode
 
When the red lock is displayed the following all non-editing actions are available. Additionally a long press on or near to an object will display the detail information screen if it is an OSM object.

### 儲存您的變更

*(需要網路連線)*

選擇您在下載時相同的按鈕或選單項目，現在選擇 "上傳資料到 OSM 的伺服器"。

Vespucci 除了支援 OAuth 的授權和標準的使用者名稱與密碼的方式。 而 OAuth 更好，因為它避免了以明文發送密碼。

New Vespucci installs will have OAuth enabled by default. On your first attempt to upload modified data, a page from the OSM website loads. After you have logged on (over an encrypted connection) you will be asked to authorize Vespucci to edit using your account. If you want to or need to authorize the OAuth access to your account before editing there is a corresponding item in the "Tools" menu.

如果您想要儲存您的工作，並且不能連入網際網路，您可以儲存成 JOSM 相容的 .osm 檔案，以後以 Vespucci 或 JOSM 任何一個上載。 

#### 在上傳解決衝突

Vespucci 有個簡單的衝突解決。不管怎樣，如果您于您的編輯察覺到有重要事件，將您的更改匯出到 .osc  檔案 (在"傳輸"選單中"匯出"的選單項目) 並且修復和上傳給 JOSM。請參閱有關詳細的説明 [衝突解決](Conflict Resolution.html)。  

## 使用 GPS

您可用 Vespucci 建立 GPX 軌跡和顯示在您的裝置上。進一步此外，您可顯示目前 GPS 位置，(在 GPS 選單中設定"顯示位置")具有螢幕中心周圍和追隨的位置，(在 GPS 選單中設定"追隨 GPS 位置")。 

如果您有設定，當用手移動螢幕或編輯將會導致停用"追隨 GPS" 模式，藍色的 GPS 箭頭將從空心變為實心箭頭。要快速的返回到"追隨"模式，只需觸碰箭頭或重新從選單中確認選項。

## 備註和錯誤

Vespucci supports downloading, commenting and closing of OSM Notes (formerly OSM Bugs) and the equivalent functionality for "Bugs" produced by the [OSMOSE quality assurance tool](http://osmose.openstreetmap.fr/en/map/). Both have to either be downloaded explicitly or you can use the auto download facility to access the items in your immediate area. Once edited or closed, you can either upload the bug or Note immediately or upload all at once.

On the map the Notes and bugs are represented by a small bug icon ![](../images/bug_open.png), green ones are closed/resolved, blue ones have been created or edited by you, and yellow indicates that it is still active and hasn't been changed. 

## 定制 Vespucci

### 設定，當您可能想要更改

* Background layer
* Overlay layer. Adding an overlay may cause issues with older devices and such with limited memory. Default: none.
* Notes/Bugs display. Open Notes and bugs will be displayed as a red bug icon, closed ones the same in green. Default: off.
* Photo layer. Displays georeferenced photographs as red camera icons, if direction information is available the icon will be rotated. Default: off.
* Node icons. Default: off.
* Keep screen on. Default: off.
* Large node drag area. Moving nodes on a device with touch input is problematic since your fingers will obscure the current position on the display. Turning this on will provide a large area which can be used for off-centre dragging (selection and other operations still use the normal touch tolerance area). Default: off.

進階參數選項

* Enable split action bar. On recent phones the action bar will be split in a top and bottom part, with the bottom bar containing the buttons. This typically allows more buttons to be displayed, however does use more of the screen. Turning this off will move the buttons to the top bar. note: you need to restart Vespucci for the change to take effect.
* Always show context menu. When turned on every selection process will show the context menu, turned off the menu is displayed only when no unambiguous selection can be determined. Default: off (used to be on).
* Enable light theme. On modern devices this is turned on by default. While you can enable it for older Android versions the style is likely to be inconsistent.
* Show statistics. Will show some statistics for debugging, not really useful. Default: off (used to be on).  

## 回報問題

如果 Vespucci 崩潰，或檢測到不一致的狀態，將會要求您發送失敗傾印。如果出現這種情況，請送出失敗傾印，但是請在每個特定的情況只要一次。如果您希望進一步的投入或對功能要求的開放議題或著類似的，請在這裡這樣做：[ Vespucci 問題追蹤](https://github.com/MarcusWolschon/osmeditor4android/issues)。如果您想討論與 Vespucci 相關的東西，您也可以在 [Vespucci google 群組](https://groups.google.com/forum/#!forum/osmeditor4android) 或是在[OpenStreetMap Android 論壇](http://forum.openstreetmap.org/viewforum.php?id=56)任何一個裡開始討論。

