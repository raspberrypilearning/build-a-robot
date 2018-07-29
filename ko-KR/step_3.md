## 로봇의 눈 만들기

로봇에게 눈을 만들어 줍시다!

+ 이 [trinket](http://jumpto.cc/web-robot)을 열어 주십시오.
    
    Trinket을 열면 아래와 같은 프로젝트가 보일 것입니다.
    
    ![screenshot](images/robot-starter.png)

이미지들은 각자 고유한 이름이나 **`id`**를 가지고 있습니다. 예를 들어, 얼굴과 눈의 이미지를 처리하는 HTML 코드(8행부터 시작하는 'face', 'eyes1', 'eye2')는 다음과 같습니다.

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

이미지의 `id`를 사용하여, CSS와 `#` 기호를 이용하면 나만의 스타일을 부여할 수 있습니다. 이 방법을 사용하면 각 이미지를 개별적으로 스타일링할 수 있습니다.

Click on the `style.css` file. Notice how the size of the robot’s face and the other images are different?

![screenshot](images/robot-id.png)

+ Add this CSS code to style the robot’s eyes:
    
        #eyes1 {
        width: 200px;
        }
        

Notice that you’re styling just the `eyes1` image, by using `#eyes1` in your CSS code. If you prefer different eyes, you can use `#eyes2` or `#eyes3` instead!

![screenshot](images/robot-eyes-width.png)

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