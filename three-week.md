# TIL
오늘 내가 배운 것들(Today I Learned)   

#### 3주차 질문
- 어제 테이블을 간단하게 만들어 달라고 해서 웹 접근성에 맞게 작성하려고 보니까 div로 되어 있는 테이블이였습니다. 이러한 경우 aria-describedby을 어떤식으로 줘야 하는지 궁금해합니다.
- 12일차에 나오는 테두리 이미지 속성인 border-image가 지원되는 웹 브라우저가 적은데 이 속성을 많이 사용하는지 
-12일차에 멀티컬럼레이아웃이 8, 9버전에서 지원이 안된다고 했는데. 만약 8,9버전도 지원해게 될때는 float로 잡아야하는지

--------------------------------------------------

#### 3주 

| 일차                    | 링크                      |
| --------------------- | ----------------------- |
| 11일차                  | <a href="#11day">클릭</a> |
| 12일차                  | <a href="#12day">클릭</a> |
| 13일차                  | <a href="#13day">클릭</a> |
| <strong>14일차</strong> | <a href="#14day">클릭</a> |
| 15일차                  | <a href="#15day">클릭</a> |

---------------------------------------------------

#### 두번째 오프라인 강의
| 제목                           | 링크                      |
| ---------------------------- | ----------------------- |
| <strong>두번째 오프라인 강의</strong> | <a href="#2week">클릭</a> |

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

<details id="12day">
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
  테두리를 이미지로 넣어줄 수 있는데 아직 많이 지원을 하지 않습니다.

    ```
    [문법]

    border-image: source [slice / width / outset] repeat]

    border-image-source
    border-image-slice

    - slice
      슬라이스는 이미지와 상, 하, 좌, 우 가장자리 오프셋을 설정합니다.
      보더 이미지를 9개 영역으로 나눌 수 있습니다.

    - width
      요소의 상/우/하/좌 테두리 이미지 너비(width)를 설정합니다. 
      실제 테두리의 영향을 받지 않고 이미지는 맨위에 배치됩니다. 
      단위 없는 값을 사용할 경우, 요소의 테두리 너비에 곱하여 오프셋합니다.

    - outset (테두리와 콘텐츠 사이 안쪽 여백 크기 조정)
      테두리 이미지를 주어진 값 만큼 패딩(안쪽) 영역을 설정합니다.
      단위 없는 값을 사용할 경우, 요소의 테두리 너비에 곱하여 오프셋합니다.

    [reqeat설정]
    - stretch (기본값) 잡아다 땡겨줍니다.
    - repeat  반복이 됩니다. (끈어진 느낌이 납니다.)
    - round   반복된 부분을 잡아 댕겨서 자연스럽게 해줍니다.
    - space

    border-image: linear-gradient(-45deg, #00b9e9, #f98b14, #503370) 20;
    ```

  #### 멀티 컬럼 레이아웃
  
  ```
  **참고
  .magazine-section:after {
    content: '';
    display: block;
    clear: both;
  }


  float로 하게 되면 디바이스의 width가 바낄때마다 길이를 조절해줘야 합니다.
  이러한 문제점을 위해 기능이 있는데요. 8버전, 9버전에서는 사용할 수 없습니다.

  실습
  .magazine-section {
    margin: 6rem 0;
    /* column-count: 4; */ 모바일 경우 찌그러지기 땜에 width를 사용.
    /* column-width: 480px; */
    columns: 320px auto -- 속경 4 auto
    동시에 설정 가능 : 320px 4

    column-gap: 2em;
    column-rule: 1px solid #dcdcdc;
  }

  컬럼의 제목같은 경우 너무 따로 노는 느낌이 드니까 column-spen: all 을 이용해 병합된 것 같은 효과를 줄 수 있음.

  컬럼 개수 또는 폭 설정
  column-count
  column-width
  columns (속기형 작성법)

  영상 강의에서는 column-count와 column-width 값을 동시 설정하지 말라고 안내했지만,
  동시 설정 가능합니다. (참고: https://goo.gl/yo1P1s)

  [예시]
  columns: 12em;       // column-width: 12em; column-count: auto
  columns: auto 12em;  // column-width: 12em; column-count: auto
  columns: 2;          // column-width: auto; column-count: 2
  columns: 2 auto;     // column-width: auto; column-count: 2
  columns: auto;       // column-width: auto; column-count: auto
  columns: auto auto;  // column-width: auto; column-count: auto
  columns: 12 320px;   // column-width: 320px; column-count: 12
     
  // 컬럼 간격 또는 구분 선 설정
  column-gap
  column-rule
  column-rule-color
  column-rule-style
  column-rule-width

  // 컬럼 병합
  column-span

  // 컬럼 채우기
  column-fill
  ```
</details>

---------------------------------------------------

<details open id="13day">
  <summary>13일차</summary>

  #### [플렉시블 레이아웃 Lecture1]   
  플로팅 포지셔닝을 배웠고 어느정도 레이아웃 구성이 되겠지만 시대는 데스크탑 시대를 벗어나고 모바일 시대로 들어가면서 21세기 기술을 사용해야 합니다.
  모던 레이아웃 중 첫번째가 플렉시블 박스입니다.
  IE를 제외한 모든 인터넷이 제공합니다. 하지만 IE에서는 사용해야할지 말아야할지 고민해야합니다.
  
  fiex-container {
    display: flex;
    flex-direction: column;
    border: 1px solid transparent;
    box-shadow: 0 0 0 1px #d9d9d9;
  }

  모든 요소들을 clearfix라는 속성을 안써도 쓴것처럼 배치가 된다.
  flex-direction 이라는 것이 중요. row - column

  플렉스 내부에 있는 것을 플렉스로 만들 수 있습니다.

  주측에 대한 정렬  
  justify-content  
  flex-start, center, flex-end, space-between, space-around  
  left, center, right, 양쪽부터 간격있게, 양쪽뛰고 간격있게.  
  flexbox-direction: row-reverse, column-reverse 반대로 정렬  
  justify-content: flex-start  

  #### [플렉시블 레이아웃 Lecture2]  
  flex-wrap: nowrap; = 계속 늘어납니다.
  flex-wrap: wrap-reverse = 위 아래 값이 교체가 됩니다.

  교차측 정렬
  align-content: center;

  가운데 정렬
  박스를 가운데 넣기 위해 line-height를 줘서 가운데로 줄 수 있지만
  justify-content: center;
  align-content: center;

  align-content: baseline; ==> 글자에 마쳐서 정렬을 해준다.


  #### [플렉시블 레이아웃 Lecture3]  
  플렉시블 레이아웃 순서 변경 order.

  align-self 자식 아이템에 대한 정렬
  align-item:nth-child(3) {
    flex: 2 0 20px;
    height: 100px;
    align-self:center;
    background: #342c40;
  }

플렉시블 참고 자료: https://heropy.blog/2018/11/24/css-flexible-box/  
</details>

---------------------------------------------------

<details open id="14day">
  <summary>14일차</summary>

  #### [그리드 레이아웃 Lecture1] 

  예전 그리드 레이아웃 방식 

  - 레이아웃 도구가 없던 시절

    예전에는 레이아웃을 위한 디자인 방법 없이 텍스트(타이포그래피) 정렬만 가능했습니다. 디자인 할 요소가 한 없이 부족했습니다.

  - 1997년 테이블 기반 레이아웃 

    테이블을 사용해서 그리드처럼 사용해왔습니다. 20년대는 목적에 맞게 사용하기 위해 더이상 테이블 레이아웃을 사용하지 않습니다. 

    테이블 기반 레이아웃은 투명한 이미지를 배경으로 만들고 그리드 레이아웃처럼 만들었는데 이러한 경우 접근성이 부재되고 의미가 상실됩니다.

    HTML 요소에 display 속성 값으로 grid를 설정하면 그리드 컨테이너가 되며, 로우와 컬럼을 가지게 된다. 
  
  - 프레임 기반 레이아웃
    
    접근성이 최악인 방식 여러장의 HTML페이지를 프레임을 사용하여 한 페이지에 결합하여 레이아웃은 만듬.

  - 플로트, 포지션 기반 레이아웃.

    웹 접근성에 대한 애기가 많아지면서 float, clear, position, Box Model 등을 사용하여 레이아웃을 만들었습니다.

    하지만 어느정도 구현이 가능하지만 비 논리적인 기법이 난무했습니다.

  - 플렉시블 박스 레이아웃 (현제)

    컨텐츠를 균듕하게 분배하고 사용 가능한 공간을 활용합니다.

    x 또는 Y축, 한쪽 방향으로만 설정 가능한 자유도가 낮은 레이아웃 기법

  - css 그리드 레이아웃

    HTML 마크업 순서와 무관하게 어디든 위치 시킬 수 있습니다. x축 y축과 다르게 내부 어디든지 위치 시킬 수 있습니다. 가장 사용하기 편리한 기법이다.

    x 그리고 Y축, 양쪽 방향 모두 설정 가능한 자유도가 높은 레이아웃 기법

  [그리드 레이아웃]
   
  그리드 레이아웃은 인터넷 익스플로어와서 지원하지 않고 edge에서는 16버전 이상이여야 지원을 합니다.

  인터넷 익스플로어 10~11 엣지 14~15 버전에는 MS라는 접두어를 붙어야 사용이 가능합니다.
  ( 브라우저 제조사의 접두사 )

  Autoprefixer는 자동으로 접두사를 붙여줍니다.

  #### [그리드 레이아웃 Lecture2] 

  [그리드 요소]
  - Grid
  HTML요소에 display속성 값으로 grid를 설정하면 그리드 컨테이너가 되며, 로우와 컬럼을 가진다. (포함된 자식 요소는 그리드 아이템이 된다.)

  - Grid Line
  그리드를 그리는 가로/세로 선을 말한다

  - Grid Track 
  수직/수평 2개의 그리드 사이에 연속된 공간을 그리드 트랙이라고 합니다.

  - Grid Cell
  4개의 그리드 라인이 모여 그려지는 공간이 그리드 셀이다.

  - Grid Area
  4개의 그리드 라인이 모여 그려지는 공간으로 셀이 묶은 영역이다.

  - Grid Gutters
  로우, 컬럼 사이 간격을 그리드 커터라고 하며, 방향에 따라 로우 거터, 컬럼 커터로 나눌 수 있다.

  - Grid Container 부모요소.
  내부에 있는 자식이 Grid Item이 되서 어디든 아이템을 배치할 수 있습니다.

  #### [그리드 레이아웃 Lecture3] 
  그리드 컨테이너 요소 설정  
  display  
    -> grid  
    -> inline-grid  
    -> ~~subgrid~~ Level2 에서 지원 예정.

  그리드 레이아웃을 짤때에는 파이어폭스에서 하는 것이 편리합니다.
  개발자 도구에서는 크롬보다 파이어폭스에서 그리드 레이아웃에 대한 기능을 더 많이 지원합니다.   

  그리드 컨테이너는 그리드 포멧팅 컨텍스트를 구축합니다. 내부에 포함된 자식 요소는 그리드 아이템이 됩니다. overflow 속성은 그리드에 적용이 가능하지만 float, clear 등 속성은 그리드 아이템에 무시됩니다.

  .grid {
    display: grid;

    /* 2행 */
    grid-template-rows: 100px 100px;

    /* 3열 */
    grid-template-columns: 150px 200px 150px;
  }

  100px의 두 행과 150px 200px 150px 의 3열이 만들어집니다.

  ```<track-size>``` 이 부분 같은 경우 그리드에서 사용 가능한 공간의 길이 입니다. (px, rex, em, %, fr, auto 등)    
  ```<line-name>``` 사용자가 설정한 임의의 선 이름

  #### [그리드 레이아웃 Lecture4] 
  [GETTER]  
  커터 속성 -> 셀의 간격
  
  /* 로우 갭(row gap) 설정 */
  grid-row-gap:10px;

  /* 컬럼 갭(column gap) 설정 */
  grid-column-gap: 10px;

  /* 속기형 갭(shortcode gap) 설정 */
  grid-gap: 10px;

  fr 경우 비율입니다. 1 1.3 1
  <유연한 길이값>

  하지만 많은 그리드의 개수들을 일일이 적게되면 계속 늘어납니다. 이러한 반복을 줄이기 위해서 그리드에서는 repeat라는 것을 지원합니다.
  repeat(3, 1fr 2fr)

  지금까지 했던 것은 명시적이였습니다.
  ```
  * CSS 그리드 레이아웃 */

  .grid {
    width: 74rem;
    
    /* 그리드 표시 (display) 설정 */
    display: grid;
    
    /* 행 템플릿 (rows template) 설정 */
    grid-template-rows: 10rem, 10rem, 10rem;
    
    /* 열 템플릿 (columns template) 설정 */
    grid-template-columns: 10rem 10rem 10rem;
    
    /* 행 그리드 거터 (row gutter, gap) 설정 */
    grid-row-gap: 1rem;
    
    /* 열 그리드 거터 (column gutter, gap) 설정 */
    grid-column-gap: 2rem;
    
    /* 그리드 거터(gutter, gap) 설정 */
    grid-gap: 1rem 3rem;
    
    /* fr(fraction, 비율) 단위 사용 */
    grid-template-rows: 1fr 1fr;
    grid-template-columns: 1fr 1.6fr 1fr;
    
    /* repeat() 함수 사용 */
    grid-template-rows:repeat(2, 1fr);
    grid-template-columns: repeat(3, 1fr);
    
    /* minmax() 함수 사용 */
  }
  ```

  #### [그리드 레이아웃 Lecture5] 
  그리드에서는 최솟값과 최대값을 설정할 수 있습니다.
  최대값과 최소값 minmax(30px, auto)

  암시적인 행렬 그리드
  grid-auto-rows
  grid-auto-columns

  미리 암시적인 행렬 그리드 값을 설정해주면 일일이 넣어줄 필요없이 자동으로 크기가 설정된다.

  /* 암시적 행, 열 그리드 트렉 사이즈 설정 */
  grid-auto-rows: minmax(10rem, auto);
  grid-auto-colums: minmax(10rem, auto)

  https://uid.gitbook.io/css-grid/
</details>

---------------------------------------------------

<details id="15day">
  <summary>15일차</summary>

  #### [그리드 레이아웃 Lecture5] 
  그리그를 그린 후에 그리드 안에 아이탬의 위치를 설정하는 방법

  - grid line
  그리드 라인을 기준으로 하여 그리드 아이템 위치를 설정할 수 있다.

  item:nth-child(1) {
    /* 그리드 아이템을 열[3,4], 행[2,3] 위치에 배치 */
    grid-column-start: 3;
    grid-column-end: 4;
    grid-row-start: 2;
    grid-row-end: 3;
  }

  grid-column: 2 / 3;
  grid-row: 3 / 4;

  Grid Span
  그리드 라인 속성에 span을 사용하여 기준 점에 상대적으로 위치 설정이 가능합니다.

  grid-row: 3 / span 2
  grid-row: span 3 / 4

  grid-area: 2 / 2 / -1 / -2
  행시작 / 행끝 / 열시작 / 열끝

  #### [그리드 레이아웃 Lecture6] 
  순서를 재설정해도 접근성에 문제가 가지 않을 때 사용합니다. 
  
  .item.itme-1 { order: 5; }
  .item.itme-1 { order: 3; }
  .item.itme-1 { order: 6; color: #a1cc2c }
  .item.itme-1 { order: 1; }
  .item.itme-1 { order: 4; }
  .item.itme-1 { order: 2; }

  grid-template-area:
    "header header header"
    "sidebar content1 content2"
    "sidebar content3 content3"
    "footer footer footer"

  #### [그리드 레이아웃 Lecture7] 

  #### [그리드 레이아웃 Lecture8] 

</details>

---------------------------------------------------


<details open id="2week">
  <summary>두번째 오프라인 강의</summary>
  저번 시간에 어떤 것을 하였는지 말씀해주셨다.

  이번 시간에 나갈 것은 헤딩이라고 하시고 순서를 말씀해 주셨는데. 나는 이게 전체 마크업에서 순서인줄 알고 잘못 이해하고 왜 저렇게 할까 라는 생각을 했는데 헤딩 마크업에 대한 순서였다.

  올래는 모바일부터하고 테스크탑으로 가는 게 베스트라고 하셨는데 데스크탑이 요소가 많아서 데스크탑부터 설명을 하고 모바일로 넘어갔다.


  스타벅스 페이지를 보게 되면 맨밑에 로고를 보게되면 이미지와 내용 링크 버튼이 있다. 그런데 스타벅스를 가까이에서 경험해보세요 x 내용입니다. 라는 것은 제목이 아니라 내용의 크기를 다르게 한것이고 이 섹션의 제목은 숨김 처리를 해야합니다.  

  header 부분을 마크업할 때 마크업 순서를 정해야합니다.

  어떤 것이 시작 부분인지 어떤 것이 마지막 부분인지 결정해야 합니다.
 
 웹 카페에 맨 위에 부분을 보게되면  맴버 처리 부분이 있는데

 ```
 로그인 | 회원가입 | 커뮤니티
 ```

 대부분 사람들이 마크업을 위에서 아래로 왼쪽에서 오른쪽으로 처리합니다.
 
 하지만 section요소인 heading을 로고에 지정하기 때문에 처음으로 해줄겁니다.

 마크업 순서
 1. 로고
 2. 링크모음 (마크업 하기 전에 사전 데이터를 도출)
 3. 폼태그 

  폼태그의 검색 버튼은 input type=search로 주게되면 알아서 구버전에서는 type을 text로 바까준다. 

responsive logos 라는 홈페이지에 들어가서 홈페이지에 이미지를 창크기를 줄이고 해서 확인 해보라고 하셨다.

개발자들은 자바스크립트로 홈페이지 사이트가 변할 때마다 이미지를 새로 가져와서 바까주기 때문에. 이미지가 별로 없는 사이트인 경우는 티가 안나지만 이미지가 많은 사이트이면 성능 저하를 가져올 수 있다.

그래서 responsive logos 사이트는 디바이스의 크기에 맞게 미디어 쿼리를 적용시켜 단위별로 웹브라우저 밖으로 나가게 해놨다.

이러한 것을 IR 기법이라고 하는데. Image Replacement 기법이라고 한다.
https://nuli.navercorp.com/sharing/blog/post/1132804

그리고 디자이너와 개발자가 싸우는 이유에 대해서 말씀해주셨다.
이것은 서로의 직무(생태계)에 대해서 전문적으로 잘 알지 못해서 생기는 문제다.

그 다음에는 맴버처리하는 부분이 a태그 앵커태그로 되어 있는데. 이 경우에는 스크린 리더가 a태그가 몇개다 라는 것처럼 말해주지 않기 때문에 
  ```
  로그인 | 회원가입 | 커뮤니티
  ```
이 링크들은 ul태그를 이용해서 몇개인지 읽게 만들어야 합니다.

그리고 가끔 ul과 li 사이에 div를 넣는 사람이 있는데 이것은 돌아가긴 하지만 올바르지 않는 시멘틱 마크업입니다.

폼태그를 묶을때는 fieldset을 사용해서 묶으면 검색봇이 legend를 보고 검색을 할 수 있습니다.

선택서식, 입력 서식을 나눠서 fieldset을 할수도 있습니다.

그리고 https://tailwindcss.com/ 타일윈드라고 있는데 이것을 사용하면 빠르게 개발을 할 수 있습니다. 그래서 비 전문가들은 빠르게 사용한 것을 간결하다고 표현하고 전공자는 공통적인 부분없이 클래스가 사용되어 이것을 간결하지 않다고 애기합니다. 인식의 차이입니다.

이미지를 넣을 때 스크린 리더가 읽을 수 있도록 alt를 이용해서 작성을 해야하는데 로고이미지라고 쓰게되면 스크린 리더는 로고 이미지 이미지라고 읽기때문에 사진의 의미를 정확히 적어야합니다.

name이란 태그 속성에 name 있는데 이것은 정보를 전송했을 때 name이라는 속성으로 파라미터가 넘어갑니다.

라벨이라는 태그를 넣어서 input태그가 어떤 것인지 설명해줬었는데 이것을 제거해야할 때에는 aria-label을 사용해서 생략 후 스크린 리더가 읽게 할 수 있다.

form 태그에 https://formspree.io/xyyzgpvy 라는 action 속성이 있는데 이 링크는 데이터 전송을 테스트 할수가 있다.

마크업을 할때에는 설계를 먼저하고 개발을 해야됩니다.

그리고 h1과 openwax 에 대해서 설명해주셨다.

이제 웹카페에 있는 헤더 부분을 그대로 복사해옵니다. h1부터 form까지. 

```
<h1 class="brand resetMargin">
  <a href="index.html">
    <img src="./images/rwd-logo.png" alt="Web Cafe">
  </a>
</h1>
<ul class="memberOnly resetList">
  <li><a href="/">로그인</a></li>
  <li><span class="divider" aria-hidden="true">ㅣ</span><a href="/">회원가입</a></li>
  <li><span class="divider" aria-hidden="true">ㅣ</span><a href="/">커뮤니티</a></li>
</ul>
<form action="https://formspree.io/xyyzgpvy" method="POST" class="searchForm">
  <fieldset class="resetBox">
    <legend>검색</legend>
    <input type="search" required placeholder="검색어를 입력하세요." name="search" aria-label="검색어">
    <button type="submit" class="button buttonSearch">검색</button>
  </fieldset>
</form>
```
공통적인 부분 추가.

```
/* 공통 Reset */
.resetMargin {
  margin: 0;
}
.resetList {
  margin: 0;
  padding-left: 0;
  list-style: none;
}
```
영어같은 경우 line-height : 1을 하게되면 짤리지 않지만 한글인 경우 line-height를 할시 1이 짤립니다.

normalize.css 노멀라이즈 CSS  
노멀라이즈 CSS 같은 경우 브라우저마다 다르게 보이는 스타일을 하나로 통힐하게 해줍니다.   
https://webdir.tistory.com/455

번역된 것들을 읽어보고 영어로 봐야겠다. 영어로 된 것을 읽으면서 공부하는 것도 나쁘지 않다고 한다.

노멀라이즈 css 다운 받을 수 있는 사이트 

https://cdnjs.com/libraries/normalize   
이 사이트로 들어가면 cdn을 다운 받을 수 있다.

cdn을 받고 맨위에 임포트를 해준다.   
@import url(https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css);

그리고 구글에 spoqa han sans 검색해서 cdn을 다운받는다.  
일본어를 쓰고 싶다면 일본어까지 넣으면 됩니다.
@import url(https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css);

옛날에는 신문의 글꼴을 전부다 이미지로 했기 때문에 외국인이 크게 유입되지 않았다. 그러자 신문 업체는 폰트자체를 글꼴로 만들어 웹폰트를 제작하니 많은 외국인 유입이 되었다.

https://webdir.tistory.com/56
cdn 말고도 @font-faced을 사용해 본트를 받을 수 있다.

@font-face {  
    font-family: 'Spoqa Han Sans';  
    font-weight: 700;  
    src: local('Spoqa Han Sans Bold'),  
    url('https://cdn.jsdelivr.net/gh/spoqa/spoqa-han-sans@01ff0283e4f36e159ffbf744b36e16ef742da6d8/Subset/SpoqaHanSans/SpoqaHanSansBold.woff2') format('woff2'),  
    url('https://cdn.jsdelivr.net/gh/spoqa/spoqa-han-sans@01ff0283e4f36e159ffbf744b36e16ef742da6d8/Subset/SpoqaHanSans/SpoqaHanSansBold.woff') format('woff'),  
    url('https://cdn.jsdelivr.net/gh/spoqa/spoqa-han-sans@01ff0283e4f36e159ffbf744b36e16ef742da6d8/Subset/SpoqaHanSans/SpoqaHanSansBold.ttf') format('truetype');  
}


</details>

<details id="2week">
  <summary>두번째 오프라인 후기</summary>
  마지막에 시간이 짧아져서 데스크탑에서 모바일로 바끼는 부분에서 설명과 코딩을 같이 강의를 하셨다. 
  
  설명을 포기하거나 코딩을 포기해서 하나에 집중해가주고 필기를 했어야했는데 둘다 가져갈려다보니 많이 놓친 부분이 많아서 저 부분에 대해서는 계속 코딩을 반복을 진행할 것이다. 
  
  오늘은 배운 것의 내용을 정리하고 내일 밀린 강의를 듣고 질문에 답하셨던 것들을 깃허브에 옮길 예정이다.

  그리고 강혜진님이 열심히 하시길래. 취업 준비생인줄 알고 회사에서 목요일날에 우리회사 주주님분들끼리 맥주를 마실때 우리 회사 프론트와 퍼블리셔를 뽑는 지 물어보았다.

  그래서 우리 회사는 프론트는 자바개발자들이 코더는 필요없고 퍼블리셔가 필요하다고 해서 

  강혜진님에게 취업 안했고 딱히 갈때가 없으시면 우리 회사 면접 한번 어떠냐고 말씀드리려고 했다. 

  그래서 쉬는 시간에 가서 명함 드리고 말씀드리니까. 이미 회사가 있다고 하신다. 디자이너 분이셨는데 취업하고 나만 열심히 공부하는 게 아니라는 것이 신기하기도 했다. 

  명함교환하고 인사를 드렸다. 명함에 연구 개발 센터라고 써졌있게 부럽기도 하고 디자인도 많이 이쁜 명함이였다.

  그리고 백엔드 개발자들한테 왜 자바스크립트를 공부하냐고 물어봤었는데.  최신 프론트 프레임워크는 제이쿼리를 지원 안한다고 들었다. 야무님이 지원을 하긴 하는데 부분적으로 지원한다고 하셨다. 

  우리 동생들 취업 준비를 위해 상담하고 스터디를 진행하고나서 너무 졸려서 자고 있어나니 9시 였다.

  밀린 동영상은 내일 봐야 할 것 같다. 항상 더 열심히 살아야겠다.

  학원이 끝나면 월세 42만원짜리 고시텔을 빼고 집에서 왔다갔다 하려고 한다.

  물론 청년전세대출 월세방을 구하기 전까지는 그렇게 다닐려고 한다.
</details>