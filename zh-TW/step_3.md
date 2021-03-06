## 給你的機器人一雙眼睛

給你的機器人裝上眼睛吧！

+ 打開[這個 trinket](http://jumpto.cc/web-robot){:target="_blank"}。
    
    檔案應該看起來像這樣︰
    
    ![截圖](images/robot-starter.png)

此專案中的每個圖案都有自己的名字（又稱為 **`id`** ）。 比方說，用來連結臉和眼睛圖案的HTML程式碼（從程式的第8行開始的 'face'、'eyes1' 和 'eyes2'）會看起來像是這樣：

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

利用 CSS 和 `#` 符號，你可以透過圖案的 `id` 為其賦與特有的樣式。這樣一來你就可以為每個圖案設計不同的樣式。

點開 `style.css` 檔案。你有注意到機器人臉和其他圖案的大小有什麼不同嗎？

![截圖](images/robot-id.png)

+ 加入這段CSS程式碼來設計機器人的眼睛：
    
        #eyes1 {
        width: 200px;
        }
        

請注意，在這段 CSS 代碼中使用的是 `#eyes1` ，也就是說你修改到的只有 `eyes1` 圖像的樣式。 如果你想讓這個機器人有不一樣的眼睛，你可以用 `#eyes2` 或 `#eyes3` 代替！

![截圖](images/robot-eyes-width.png)

你注意到每個圖案是如何按照程式顯示出來的嗎？ 這叫做**相對（relative）**位置。 如果你想明確地告訴瀏覽器將機器人的眼睛放在哪裡，就需要使用**絕對（absolute）**位置。

+ 將這三行代碼加到 `eyes1` 圖案的 CSS 代碼裡：
    
        position: absolute;
        top: 200px;
        left: 100px;
        

你應該會看見機器人的眼睛移動到了正確的位置。

![截圖](images/robot-eyes-position.png)

這三行CSS程式碼告訴了瀏覽器從網頁的左上角算起來，要距離多遠顯示圖案。

![截圖](images/robot-eyes-position2.png)

你也可以用 `bottom` 而不是 `top` 來告訴瀏覽器從畫面底部算起的距離，或者把 `left` 改成 `right`，告訴瀏覽器從從畫面的右側算起。