## Poner ojos a tu robot

¡Vamos a poner ojos a tu robot!

+ Abre [este trinket](http://jumpto.cc/web-robot).
    
    El proyecto debería parecerse a esto:
    
    ![captura de pantalla](images/robot-starter.png)

Cada imagen en este proyecto tiene su proprio nombre (o **`id`**). Por ejemplo, el código HTML para los imágenes de la cara y los ojos (‘face’, ‘eyes1’, y ‘eyes2’, a partir de la línea 8 de tu código) se parece a esto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Puedes usar el `id` de una imagen para darle su propio estilo, usando CSS y el símbolo `#`. Esto te permite diseñar cada imagen por separado.

Haga clic en el fichero `style.css`. ¿Observas que el tamaño de la cara del robot y las otras imágenes son diferentes?

![captura de pantalla](images/robot-id.png)

+ Añade este código CSS para diseñar los ojos del robot:
    
        #eyes1 {
        width: 200px;
        }
        

Ten en cuenta que estás diseñando solo la imagen `eyes1`, usando `#eyes1` en tu código CSS. ¡Si prefieres ojos diferentes, puedes usar `#eyes2` o `#eyes3`!

![captura de pantalla](images/robot-eyes-width.png)

¿Observas que las imágenes se muestran una tras otra? Esto se llama posicionamiento **relativo**. Si quieres decirle al navegador exactamente donde colocar los ojos de tu robot, deberás usar posicionamiento **absoluto** en su lugar.

+ Añade estas tres líneas al código CSS para tu imagen `eyes1`:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

Deberías ver que los ojos de tu robot se mueven al lugar correcto en tu robot.

![captura de pantalla](images/robot-eyes-position.png)

Este código CSS indica al navegador lo lejos de la esquina superior izquierda de la página web que debe aparecer la imagen.

![captura de pantalla](images/robot-eyes-position2.png)

Puedes usar `bottom` en lugar de `top` para indicar al navegador lo lejos de la parte inferior de la pantalla que debe aparecer la imagen, así como `right` en lugar de `left`.