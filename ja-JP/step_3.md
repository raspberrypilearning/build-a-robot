## ロボットの目を作る

ロボットの目を作ろう!

+ [ここ](http://jumpto.cc/web-robot)を開く
    
    プロジェクトはこのようになります。
    
    ![screenshot](images/robot-starter.png)

このプロジェクトの各イメージにはそれぞれに名前(または**`id`**)があります。 たとえば、顔と目のイメージ(あなたのコードの8行目から始まる‘face’, ‘eyes1’, ‘eyes2')に対応するHTMLコードは次のとおりです。

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

CSSと`#`シンボルを使って独自のスタイルを設定するため、イメージの`id`を使用できます。これは、それぞれ個別にイメージのスタイルを設定できます。

`style.css`ファイルをクリックします。どれくらいロボットの顔と他のイメージのサイズが違っているか注目してください。

![screenshot](images/robot-id.png)

+ このCSSコードを追加してロボットの目のスタイルを設定します。
    
        #eyes1 {
          width: 200px;
        }
        

あなたのCSSコードで`#eyes1`を使うことで`eyes1`イメージのスタイルを設定していることに注目してください。 もし違った目をお望みなら、`#eyes2`または`#eyes3`を代わりに使うことができます。

![screenshot](images/robot-eyes-width.png)

それぞれのイメージがどのように次々と表示されるか注目ください。 これは**相対的な**ポジショニングと呼ばれています。 If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.