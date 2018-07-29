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

`style.css` 파일을 클릭해 주십시오. 로봇의 얼굴 이미지와 다른 이미지들의 크기는 서로 다릅니다. 이게 어떻게 가능한 걸까요?

![screenshot](images/robot-id.png)

+ 아래의 CSS 코드로 로봇의 눈을 스타일링합니다.
    
        #eyes1 {
        width: 200px;
        }
        

당신은 `eyes1` 이미지만 스타일링하고 있다는 점에 주목해 주십시오. CSS 코드 안에서 `#eyes1`을 사용하기 때문입니다. 다른 눈들이 더 좋다면 `#eyes1` 대신 `#eyes2` 나 `#eyes3`을 사용할 수도 있습니다.

![screenshot](images/robot-eyes-width.png)

이미지들이 각각 어떻게 보이는지에 주목해 주십시오. 이것을 **상대적** 위치라고 합니다. 만약 브라우저에 로봇의 눈을 배치할 위치를 정확하게 지정하고 싶다면, 상대적 위치 대신 **절대적** 위치를 사용해야 합니다.

+ 아래의 CSS 코드 세 줄을 `eyes1` 이미지의 코드에 추가해 주십시오.
    
        position: absolute;
        top: 200px;
        left: 100px;
        

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](images/robot-eyes-position.png)

This CSS code tells the browser how far from the top left-hand corner of the webpage to display the image.

![screenshot](images/robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as `right` instead of `left`.