## Give your robot eyes

--- task ---

Open the <a href="https://editor.raspberrypi.org/en/projects/build-a-robot-starter" target="_blank">starter project</a>.

--- /task ---

Each image in this project has its own name (or **`id`**). For example, the HTML code to address the face and eye images (‘face’, ‘eyes1’, and ‘eyes2’, starting on line 8 of your code) looks like this:

--- code ---
---
language: html
filename: 
line_numbers: true
line_number_start: 8
line_highlights:
---
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>

--- /code ---

You can use an image’s `id` to give it its own style, using CSS and the `#` symbol. This allows you to style each image separately.

--- task ---

Open the `style.css` file. 

Notice how the size of the robot’s face and the other images are different.

--- /task ---


--- task ---

Add this CSS code to style the robot’s eyes:

--- code ---
---
language: css
filename: 
line_numbers: 
line_number_start: 
line_highlights:
---
#eyes1 {
    width: 200px;
    }

--- /code ---

**Note**: You are styling just the `eyes1` image, by using `#eyes1` in your CSS code. If you prefer different eyes, you can use `#eyes2` or `#eyes3` instead!

--- /task ---

Notice how each image is displayed one after the other? This is called __relative__ positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use __absolute__ positioning instead.

--- task ---

Add these three lines to the CSS code for your `eyes1` image:

--- code ---
---
language: css
filename: 
line_numbers: 
line_number_start: 
line_highlights: 3 - 5
---
#eyes1 {
    width: 200px;
    position: absolute;
    top: 200px;
    left: 100px;
    }
    
--- /code ---

--- /task ---

You should see that your robot’s eyes move to the correct place on your robot.

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![The robot head with arrows indicating how far the eye is positioned from the top (200px) and left (100px).](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.
