## Giving your robot eyes

Let’s give your robot some eyes!


+ Open this trinket: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>.

    The project should look like this:

	![screenshot](images/robot-starter.png)

Each image in this project has it’s own name (or __id__). For example, the HTML for the face and eye images (‘face’, ‘eyes1’ and ‘eyes2’ starting on line 8 of your code) looks like this:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

You can use an image’s id to give it it’s own style, by using the `#` symbol. This allows you to style each image separately.

Click on the `style.css` file. Notice how the size of the robot’s face and the other images are different?

![screenshot](images/robot-id.png)

+ Add this CSS code to style the robot’s eyes:

    ```
    #eyes1 {
    width: 200px;
    }
    ```

Notice that you’re styling just the `eyes1` image, by using `#eyes1` in your CSS. If you prefer, you can use `#eyes2` or `#eyes3` instead!

![screenshot](images/robot-eyes-width.png)

Notice how each image is displayed one after the other? This is called __relative__ positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use __absolute__ positioning instead.

+ Add these 3 lines of code to the CSS for your `eyes1` image:

    ```
    position: absolute;
    top: 200px;
    left: 100px;
    ```

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top / left of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as using `right` instead of `left`.

