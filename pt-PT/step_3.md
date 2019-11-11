## Dando olhos ao teu robô

Vamos dar olhos ao teu robô!

+ Abre [este trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    O projeto deverá parecer-se com isto:
    
    ![screenshot](images/robot-starter.png)

Cada imagem neste projeto tem o seu próprio nome (ou **`id`**). Por exemplo, o código HTML para endereçar as imagens do rosto e olhos ('face', 'eyes1' e 'eyes2', iniciando na linha 8 do teu código) tem a seguinte aparência:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Podes usar o `ID` de uma imagem para lhe dares o seu próprio estilo, usando CSS e o símbolo ` # `. Isso permite que possas estilizar cada imagem separadamente.

Clica no ficheiro ` style.css `. Observas como o tamanho do rosto do robô e as outras imagens são diferentes?

![screenshot](images/robot-id.png)

+ Adiciona este código CSS para estilizar os olhos do robô:
    
        # eyes1 {
        width: 200px;
        }
        

Nota que estás a estilar apenas a imagem `eyes1`, ao usar `#eyes1` no teu código CSS. Se preferires olhos diferentes, podes usar ` # eyes2 ` ou ` # eyes3 `!

![screenshot](images/robot-eyes-width.png)

Notas como cada imagem é exibida uma após a outra? Isto é chamado posicionamento **relativo**. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.