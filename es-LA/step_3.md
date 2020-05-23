## Giving your robot eyes

¡Vamos a darle ojos a tu robot!

+ Abre [this trinket](http://jumpto.cc/web-robot){:target="_blank"}.
    
    El proyecto debe verse así:
    
    ![captura de pantalla](images/robot-starter.png)

Cada imagen en este proyecto tiene su proprio nombre (or **`id`**). Por ejemplo, el código HTML para dirigirse a las imágenes de la cara y los ojos (‘face’, ‘eyes1’, y ‘eyes2’, a partir de la línea 8 de tu código) se parece a esto:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Puedes usar el `id` de una imagen para darle su propio estilo, usando CSS y el símbolo `#`. Esto te permite diseñar cada imagen por separado.

Haga clic en el archivo `style.css`. ¿Observas cómo el tamaño de la cara del robot y las otras imágenes son diferentes?

![captura de pantalla](images/robot-id.png)

+ Agrega este código CSS para diseñar los ojos del robot:
    
        #eyes1 {
        width: 200px;
        }
        

Ten en cuenta que estás diseñando solo la imagen `eyes1`, usando `#eyes1` en tu código CSS. ¡Si prefieres ojos diferentes, puedes usar `#eyes2` o `#eyes3` en su lugar!

![captura de pantalla](images/robot-eyes-width.png)

Notice how each image is displayed one after the other? This is called **relative** positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use **absolute** positioning instead.

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.