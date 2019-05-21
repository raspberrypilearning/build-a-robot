## Dando olhos ao seu robô

Vamos dar olhos ao seu robô!

+ Open [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    O projeto deve ficar assim:
    
    ![screenshot](images/robot-starter.png)

Cada imagem neste projeto tem seu próprio nome (ou **`id`**). Por exemplo, o código HTML para endereçar as imagens de rosto e olhos ('face', 'eyes1' e 'eyes2', iniciando na linha 8 do seu código) se parece com isto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Voce pode usar o `id` da imagem para dar um estilo próprio, usando o CSS e o símbolo `#`. Isto permite que você modifique cada imagem separadamente.

Clique no arquivo `style.css`. Percebe como o tamanho do rosto do robô e as outras imagens são diferentes?

![screenshot](images/robot-id.png)

+ Adicione este código CSS para estilizar os olhos do robô:
    
        #eyes1 {
        width: 200px;
        }
        

Observe que você está modificando apenas a imagem do `eyes1`, usando `#eyes1` no seu código CSS. Se você preferir olhos diferentes, você pode usar `#eyes2` ou `#eyes3`!

![screenshot](images/robot-eyes-width.png)

Percebe como cada imagem é exibida uma após a outra? Isso é chamado de posicionamento **relativo**. Se você quiser dizer ao navegador exatamente onde colocar os olhos do seu robô, você vai precisar usar posicionamento **absoluto**.

+ Adicione estas três linhas ao código CSS para a sua imagem `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Você verá que os olhos do seu robô se movem para o lugar descrito.

![screenshot](images/robot-eyes-position.png)

Este código CSS informa ao navegador a que distância do canto superior esquerdo da página da Web deve exibir a imagem.

![screenshot](imagens/robot-eyes-position2.png)

Você pode usar `bottom` ao invés de `top` para dizer ao navegador o quão longe da parte inferior da tela deve mostrar a imagem, bem como `right` ao invés de `left`.