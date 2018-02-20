## Poner ojos en tu robot

¡Vamos a poner ojos en tu robot!

+ Abre [este trinket](http://jumpto.cc/web-robot).
    
    El proyecto debería parecerse a esto:
    
    ![captura de pantalla](images/robot-starter.png)

Cada imagen en este proyecto tiene su proprio nombre (o **`id`**). Por ejemplo, el código HTML para los imagenes de la cara y los ojos (‘face’, ‘eyes1’, and ‘eyes2’, a partir de línea 8 de tu código) se parece a esto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Puedes usar la `id` de una imagen para darla su propio estilo, usando CSS y el símbolo ` # `. Esto te permite diseñar cada imagen por separado.

Haga clic en el fichero `style.css`. ¿Observas que el tamaño de la cara del robot y las otras imágenes son diferentes?

![captura de pantalla](images/robot-id.png)

+ Añade este código CSS para diseñar los ojos del robot:
    
        #eyes1 {
        width: 200px;
        }
        

Ten en cuenta que estás diseñando solo la imagen `eyes1`, usando `#eyes1` en tu código CSS. ¡Si prefieres ojos diferentes, puedes usar `#eyes2` o `#eyes3`!

![captura de pantalla](images/robot-eyes-width.png)

¿Observas que las imágenes se visualizan una tras otra? Esto se llama posicionamiento **relative**. Si quieres decir el navegador exactamente dónde colocar los ojos de tu robot, deberás usar posionionamiento **absolute** en su lugar.

+ Añade estas tres líneas al código CSS para su imagen `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Deberías ver que los ojos de tu robot se mueven al lugar correcto en tu robot.

![captura de pantalla](images/robot-eyes-position.png)

Este código CSS indica al navegador qué tan lejos de la esquina superior izquierda de la página web debe aparecer la imagen.

![captura de pantalla](images/robot-eyes-position2.png)

Puedes usar `bottom` en lugar de `top` para indicar al navegador qué tan lejos de la parte inferior de la pantalla debe aparecer la imagen, así como `right` en lugar de `left`.