## 给你的机器人装上眼睛

让我们来给你的机器人装上眼睛！

+ 打开[该饰品](http://jumpto.cc/web-robot)。
    
    效果应该是这样：
    
    ![screenshot](images/robot-starter.png)

此项目中每张图像都有它自己的名称（或**`ID`**） 例如，代表面部和眼睛图像的HTML代码（从代码的第8行开始的“face”，“eyes1”和“eyes2”）如下所示：

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

你可以使用CSS和`#`符号来为图像设计出你自己的风格`ID`。你可以单独设计每个图像的样式。

点击该文件`style.css`。注意到机器人脸部的大小和其它图像的大小有什么不同吗？

![screenshot](images/robot-id.png)

+ 添加这行CSS代码来设计机器人的眼睛：
    
        #eyes1 {
        width：200px; 
        }
        

请注意，这行CSS代码中使用`#eyes1`只有改到 `eyes1`图片的样式哦。 如果你更喜欢让机器人拥有不同的双眼，你可以用`#eyes2`或`#eyes3`代替！

![screenshot](images/robot-eyes-width.png)

注意到每张图像是如何显示的吗？ 这叫做**相对**定位。 如果你想让浏览器将机器人的眼睛明确地放在某处，你就需要使用**绝对**定位。

+ Add these three lines to the CSS code for your `eyes1` image:
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.