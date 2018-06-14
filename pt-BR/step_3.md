## Dando olhos ao seu robô

Vamos dar alguns olhos ao seu robô!

+ Abra [este trinket](http://jumpto.cc/web-robot).
    
    O projeto deve ficar assim:
    
    ![screenshot](images/robot-starter.png)

Cada imagem neste projeto tem seu próprio nome (ou **`id`**). Por exemplo, o código HTML para endereçar as imagens de rosto e olhos ('face', 'eyes1' e 'eyes2', iniciando na linha 8 do seu código) se parece com isto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Voce pode usar o `id` da imagem para dar um estilo próprio, usando o CSS e o símbolo `#`. Isto permite que você estilize cada imagem separadamente.

Clique no arquivo `style.css`. Percebe como o tamanho do rosto do robô e as outras imagens são diferentes?

![screenshot](images/robot-id.png)

+ Adicione este código CSS para estilizar os olhos do robô:
    
        #eyes1 {
        width: 200px;
        }
        

Observe que você está estilizando apenas a imagem do `eyes1`, usando `#eyes1` no seu código CSS. Se você preferir olhos diferentes, você pode usar `#eyes2` ou `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Percebe como cada imagem é exibida uma após a outra? Isso é chamado de posicionamento **relativo**. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.