# TIL
오늘 내가 배운 것들(Today I Learned)   

#### 3주차 질문
- 어제 테이블을 간단하게 만들어 달라고 해서 웹 접근성에 맞게 작성하려고 보니까 div로 되어 있는 테이블이였습니다. 이러한 경우 aria-describedby을 어떤식으로 줘야 하는지 궁금해합니다.

--------------------------------------------------

#### 3주 

| 일차   | 링크                      |
| ---- | ----------------------- |
| 11일차 | <a href="#11day">클릭</a> |
| 12일차 | <a href="#12day">클릭</a> |
| 13일차 | <a href="#13day">클릭</a> |
| 14일차 | <a href="#14day">클릭</a> |
| 15일차 | <a href="#15day">클릭</a> |

---------------------------------------------------
<details id="11day">
  <summary>11일차</summary>

  #### [2D 트랜스폼]   
  뷰포트의 너비값과 높이값 (vh, vx)
  ```
  height {
    height: 100vh; -> 사용자가 보는 화면 vh
  }
  ```

  2D 트랜스폼 
  ```
  // 회전 
  rotateX()
  rotateY()
  rotate(x, y)

  // 크기 
  scaleX()
  scaleY()
  scale(x, y)
  
  // 이동
  translateX()
  translateY()
  translate(x, y)

  // 비틈
  skewX()
  skewY()
  ```

  예제
  ```
  .handline {
    position: absolute;
    top: 100px;
    left: 50%;
    margin-left: -156px;
    transform: rotate(0deg); /* degree각도, 라디안: radian */
    transform: rotate(0.5turn); /* 반바퀴 회전 */
  }

  .sonic-adventure {
    position: relative;
    background: #ffff00;
    height: inherit;     -- 부모 요소로 부터 높이 상속 
  }

  .headline {
    position: absolute;
    top: 100px;
    left: 50%;
    margin-left: -156px;
  }

  .sonic {
    position: absolute;
    bottom: 120px;
    left: 50%;
    margin-left: -136.5px;
    transform-origin: 0% 0%; -- 중심충 교체
    transform: scale(1.2) translateX(-40px) translateY(-140px) rotate(10deg)

  }

  .desc {
    position: absolute;
    top: 480px;
    transform: rotate(-80deg) translate(180px, 90px);
    width: 280px;
    text-align: right;
    color: #005baa;
  }
  ```


  #### [트랜지션]  
  
  CSS 트랜지션(Transition): IE 10+
  ```
  transition-property       트랜지션 속성
  transtion-duration        트랜지션 시간
  transtion-timing-function 트랜지션 타이밍 함수
  transtion-delay           트랜지션 지연시간
  transition                트랜지션 속기형
  ```

  ```
  .headline {
    position: absolute;
    top: 40px;
    left: 50%;
    margin-left: -156px;
    transition-property: top, transform;
    transition-duration: 0.45s, 0.8s;
    /* transition-timing-function: lineor */
     transition-timing-function: cubic-bezier(0.895, 0.030, 0.685, 0.220); /* easeInQuart */
    transition-delay: 0.4s, 0.4s;
  }

  .sonic-adventure:hover .headline {
    /* 종료상태 (final state) */
    top: 100px;
    transform: rotate(10deg);
  }
  ```

  easeInOutCubic을 사용하기 위해서는 Compass Ceaser 플러그인을 사용해야합니다.
  https://matthewlein.com/tools/ceaser
  해당 transtion 속도를 보여주는 사이트
  easings.net

  외우기에는 힘들기 때문에 가져다가 사용해야 됩니다.
  
  ```
  사용할 수 있는 타임함수들은 line, ease, ease-in, ease-out, ease-in-out가 있습니다.
  이것 이외의 속성은 큐빅베이저라는 속성을 써야합니다. 시저라는 홈페이지에서 사용.
  ```

  ```
  transition 사용법
  transition: top 0.4 ease, transform 0.6s ease-in-out 0.4s;
  
  모든 것의 애니메이션을 줄때
  transition: all 0.4s ease-out 0.32s;
  ```
  이야 이쁘다;
  https://codepen.io/yamoo9/full/qoOGdg

  #### [애니메이션]    

  애니메이션(Animation)
  ```
  animation-name            애니메이션 이름
  animation-duration        애니메이션 시간
  animation-timing-function 애니메이션 타이밍 함수
  animation-delay           애니메이션 지연시간
  animation-direction       애니메이션 종료 후, 진행 (순/역) 방향
  animation-iteration-count 애니메이션 반복 횟수 (infinite: 무한반복)
  animation-play-state      애니메이션 재생 / 일시정지 설정
  animation-fill-mode       애니메이션 시작 전/종료 후 키프레임 설정 (forwards: 유지)
  animation                 애니메이션 속기형

  .sonic {
    position: absolute;
    bottom: 10px;
    left: 10px;
    width: 100px;
    height: auto;
    animation-name: sonic-running;
    animation-duration: 1s;
    animation-timing-function: linear;
    animation-iteration-count: 2; -- 무한 반복 infinite
    animation-direction: alternate;
    animation-fill-mode: forwords -- backwards
    animation-delay: 400ms;
  }

  .sonic {
    position: absolute;
    bottom: 10px;
    left: 10px;
    width: 100px;
    height: auto;
    animation: 
      0.5s
      ease-in
      forwards
      0.2s;
  }


  .sonic-adventure:active .sonic {
    animation-play-state: paused;
  }

  .sonic.is-run  { animation-name: sonic-running }
  .sonic.is-jump { animation-name: sonic-jump }


  /* 애니메이션 정의 */
  @keyframes sonic-running {
    to {
      transform: translateX(740px);
    }
  }

  @keyframes sonic-jump {
    50% {
      transform: translateY(-140px);
    }
    100% {
      transform: translateY(0);
    }
  }
  ```
  애니메이션 사용법
  https://developer.mozilla.org/ko/docs/Web/CSS/animation


  #### [3D 트랜스폼]   

  ```
  CSS 3D 트랜스폼(Transforms)
  
  <트랜스폼을 적용할 요소에 적용 하는 속성>
 
  transform-origin
  backface-visibility
 
  회전 시키는 부분
  rotateX()
  rotateY()
  rotateZ()
  rotate3d()
  
  위치이동
  translateX()
  translateY()
  translateZ()
  translate3d()
 
  확대
  scaleX()
  scaleY()
  scaleZ()
  scale3d()
 
  비틀기
  skewX()
  skewY()
  skew()

  perspective 원근
  
  <자식 요소를 3D 처리할 부모 요소에 설정>
 
  perspective
  perspective-origin
  transform-style: preserve-3d (요소의 자식이 3D 공간에 배치)
 
  ```
  3D 트랜스폼 같은 경우 어려워서 여러번 공부를 해야할 것같다.
  https://webclub.tistory.com/622

</details>

---------------------------------------------------

<details open id="12day">
  <summary>12일차</summary>

  #### [그레디언트] 

  ```
  overflow-x: hidden;
  min-height: 100vh;
  /*
    yellow:            #f7e763
    dark-yellow:       #5d5a40
    orange:            #fe8201
    orange-red:        #ff3400
    dark-orange:       #64471d
    blue-violet:       #6c52da
    dark-blue-violet:  #3a2c76
    cyan:              #45d5bf
    dark-cyan:         #1f685d
    black:             #2e2f32
   */
  background: #ff3400;
  
  /* 선형 그레디언트 ----------------------------- */
  
  background: linear-gradient(180deg, #ff3400, #f7e763);
  https://aboooks.tistory.com/362 - gradient에 대한 설명
  to left, to right, to top, to bottom

  만약 가운데 색깔을 추가하고 싶다면 왼쪽 가운데 오른쪽 순으로 적어주면 됨.
  background: linear-gradient(45deg, #ff3400, #45d5bf, #f7e763);

  퍼센트를 주게 되면 퍼센트만큼 색을 받을 수 있음.
  background: linear-gradient(
    45deg, 
    #6c52da 25%,
    #ff3400 25%, 
    #ff3400 50%, 
    #45d5bf 50%,
    #45d5bf 75%,
    #f7e763 75%,
    #f7e763
  );

  -> 하지만 세밀한 각도를 위해서 deg로 잡아주는게 중요하다고 생각합니다.

  /* 원형 그레디언트 ----------------------------- */
  기존적인 문법은 동일.
  background: radial-gradient(#6c52da 50%, #2e2f32 50%);

  세로가 너무 길어서 타원형태로 나올때 circle이라는 것을 적어주면 됨
  background: radial-gradient(circle,#6c52da 50%, #2e2f32 50%);

  이것도 동일하게 색깔을 지정할 수 있습니다.
  background: radial-gradient(circle, #f7e763 25%,#6c52da 25%, #6c52da 50%,#2e2f32 50%);

  background: radial-gradient(
    circle closest-side, // farthest-corner 기본값 (가장멀리있는 코너까지 확장)
    #f7e763,
    #6c52da,
    #2e2f32);

  /* 배경 패턴 --------------------------------- */
  /* url("//goo.gl/B6SfbX") */
  background: url("//goo.gl/B6SfbX")
  background-size: 90px;

  /* 오버레이 그레디언트 -------------------------- */
  /* 멀티 배경 테크닉 활용 */
   background: 
    linear-gradient(45deg, hsla(12, 100%, 50%, 0.2), hala(54, 90%, 68% 0.2)),
    url("//goo.gl/B6SfbX")
    background-size: contain, 120px;

  contain : 배경을 사용하는 요소를 벗어나지 않는 최대 크기로 이미지를 확대 또는 축소합니다. 가로 세로 비율을 유지합니다.

  /* 멀티 그레디언트 ----------------------------- */
  background:
    radial-gradient(circle at 50% 0, rgba(255,0,0,0.45), rgba(255,0,0,0) 65.70%)
    radial-gradient(circle at 6.7% 75%, rgba(0,255,0,0.45), rgba(255,0,0,0) 65.70%)
    radial-gradient(circle at 93.3% 75%, rgba(0,0,255,0.45), rgba(255,0,0,0) 65.70%)
    url("//goo.gl/B6SfbX")
  /* 반복 그레디언트 ----------------------------- */
  background: repeating-linear-gradient(
    -45deg,
    #f7e763,
    #f7e763 10px,
    #5d5a40 10px,
    #5d5a40 20px
  );
  background: repeating-radial-gradient(
    circle at 50% 50%,
    #f7e763,
    #f7e763 10px,
    #5d5a40 10px,
    #5d5a40 20px
  );

  박스 그림자 설정
  box-shadow: 0 0 0 1px #3f3f3f;

  둥근 테두리 설정
  border-radius: 170px 0 0 170px;
  border-radius: 6px;

  **
  광택 효과 설정
  background:
    linear-gradient(
      148deg,
      rgba(255, 255, 255, 0) 20%,
      rgba(255, 255, 255, 0.15) 47%,
      rgba(255, 255, 255, 0.3) 47%,
      rgba(255, 255, 255, 0.3) 47.1%,
      transparent 47.1%
    )
  ```  

  #### [보더 이미지]  

  #### [멀티 컬럼 레이아웃]    

</details>

---------------------------------------------------

<details id="13day">
  <summary>13일차</summary>

  #### [플렉시블 레이아웃 Lecture1]   

  #### [플렉시블 레이아웃 Lecture2]  

  #### [플렉시블 레이아웃 Lecture3]  

</details>

---------------------------------------------------

<details id="14day">
  <summary>14일차</summary>

  #### [그리드 레이아웃 Lecture1]   

  #### [그리드 레이아웃 Lecture2] 

  #### [그리드 레이아웃 Lecture3] 

  #### [그리드 레이아웃 Lecture4] 

</details>

---------------------------------------------------

<details id="15day">
  <summary>15일차</summary>

  #### [그리드 레이아웃 Lecture5] 

  #### [그리드 레이아웃 Lecture6] 

  #### [그리드 레이아웃 Lecture7] 

  #### [그리드 레이아웃 Lecture8] 

</details>

---------------------------------------------------