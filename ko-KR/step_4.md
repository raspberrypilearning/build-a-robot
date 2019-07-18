## 로봇의 입 만들기

로봇에게 입을 만들어 줍시다!

- 이 CSS 코드를 `style.css`의 가장 아래쪽에 추가해 주십시오. 이 코드는 `mouth1` 이미지를 스타일링합니다.
    
        #mouth1 {
            width: 50px;
            position: absolute;
            top: 200px;
            left: 200px;
        }
        

그런데 로봇의 입이 너무 작은데다, 위치까지 부적절하네요!

![스크린샷](images/robot-mouth.png)

- CSS 코드를 수정하여 이 문제를 해결해 볼까요?

\--- hints \--- \--- hint \--- `style.css` 파일의 `mouth1` 안에서, `width`로 너비를, `top`, `left`로 위치를 변경하면 이 문제를 해결할 수 있습니다.

원하는 모양이 나올 때까지 여러 값들을 시도해 봅시다. \--- /hint \--- \--- hint \--- 당신은 다음과 같은 것을 만들어야 됩니다.

![스크린샷](images/robot-mouth-code.png) \--- /hint \--- \--- /hints \---