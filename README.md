# TIL
오늘 내가 배운 것들(Today I Learned)   

#### 4주차 질문

--------------------------------------------------

#### 4주 

| 일차                    | 링크                      |
| --------------------- | ----------------------- |
| <strong>16일차</strong> | <a href="#16day">클릭</a> |
| 17일차                  | <a href="#17day">클릭</a> |
| 18일차                  | <a href="#18day">클릭</a> |
| 19일차                  | <a href="#19day">클릭</a> |
| 20일차                  | <a href="#20day">클릭</a> |

---------------------------------------------------



<details open id="16day">
  <summary>16일차</summary>

  #### 반응형 웹이란? (RWD)
  Responsive Web Design -> 반응형 웹 디자인  
  과거를 답습하는 것은 이제 그만! 

  답습 => 전부터 해 내려오거나 있던 방식이나 수법을 비판적으로 검토하지 않고, 있는  그대로 받아들이거나 따름.  
  원래그랬어? 실무에서 많이 말하는데 원래 그런 것은 없습니다.  
  
  이세대가 필요하는 기술을 가지고 클라이언트의 요구사항을 구현해 내는 것이 필요합니다.

  오늘을 연구하고 만들어야 합니다. 사용자의 인터페이스 환경을 여러분이 만들어 내는 것이 필요합니다. 테크놀로지의 반전으로 월드 와이드 웹은 데스크톱을 벗어나 세상 모든 기기에서 이용 가능해졌다.

  우리가 만들어야하는 것은 서비스고 서비스는 사용자에게 제공되는 내용 콘텐츠와 컨텍스트 입니다. 

  테크놀로지의 발전은 디자인 바운더리를 변경시켰습니다. 제한된 환경에서 벗어나 무한대의 환경으로 진화되고 있는 것이 웹이다.

  그 안에 들어가는 설계를 우리가 해야한다. 사용자의 경험을 유연하게 확장 시켜야 한다.

  컨텐츠는 물과 같고 어떤 용기에 담든 성질은 똑같다.

  반응형 웹 시대를 위한 디자인. 다양한 디바이스에 사용자에게 제공하는 컨텐츠를 담아내는 것. 

  반응형 웹 디자인이란? 사용자의 환경(스크린 사이즈, 플랫폼, 회전방향 등)을 고려하여 응답할 수 있도록 제작하는 것을 말한다.

  2010년 Ethan Marcotte 반응형웹 => 디바이스에서 콘텐츠를 감추거나 격리시키는 것보다 최적화된 뷰를 사용자에게 제공하여 콘텐츠를 효율적으로 담는 것이 우리가 수행해야 할 일입니다.

  #### 콘텐츠 구성 
  
  반응형 웹 프로젝트를 시작하기 전 무엇을 고려하고, 알아야 할까?

  ```
  1. 콘텐츠 전략 (Content strategy)
  2. 유연한 그리드 레이아웃 (Flexible grid layout)
  3. 유연한 이미지 / 미디어 (Flexible images and media)
  4. 디바이스 픽셀 밀도 (Device Pixel Density)
  5. 중단점 / 미디어 쿼리 (Breakpoint and Media queries)
  ```

  [콘텐츠 전략]
  콘텐츠의 구조를 치밀하게 분석하지 않고는 좋은 사용자 경험을 제공하기 어렵다.
  고정된 가로 폭과 해상도에서 콘텐츠가 영구적으로 자리 잡았던 디자인은 과거의 것이 되었다. 다양하게 변화되는 가로 폭과 해상도에 최적의 경험을 제공할 수 있는 무용술이 필요로 한다.

  [콘텐츠 쌓임]
  4컬럼 레이아웃 디자인의 화면 폭이 줄어들 경우 쌓이는 것은 불가피하다. 4->3->2->1
  하지만 중요한 정보가 1번이 아닐 수가 있다.

  [콘텐츠 순서]
  중요한 컨텐츠는 우선적으로 보여야 합니다. 크기가 작은 모바일 환경에서 우선적으로 보여져야 할 콘텐츠가 무엇인지 고려해야 함을 말한다.

  [콘텐츠 맞물림]
  상황에 따라서는 순서가 뒤섞이는 구조로 보여야한다. float나 position이 아닌 플렉시블 같은 레이아웃 기술을 사용해야한다. 

  [플렉시블 박스]
  콘텐츠 중심 전략, 콘텐츠 구성(안무법)등을 원활하게 구현하기 위한 새로운 레이아웃 기술이 요구되었다.

  #### 유연한 그리드
  RWD에서는 픽셀이 아닌, 상대 단위를 사용해야 하기에 픽셀을 상대 단위로 바꾸는 계산식을 사용해야 한다. 
  그리드 퍼센트  (전체PX / 현제PX) X 100

  [테크니컬 이슈]
  물처럼 흐르는 유연한 레이아웃을 구현할 경우 발생하는 테크니컬 이슈는 정확하게 정수로 떨어지지 않는 픽셀의 경우 각각 브라우저가 처리하는 방식이 달라서 퍼센트 값을 픽셀로 변경하는 과정이 발생한다.

  // 보충

  #### 유연한 이미지
  이미지를 포함하는 컨테이너 요소의 폭에 맞쳐 크기가 변경되는 이미지를 말한다. 

  콘텐츠 이미지   
  width: 100%;
  height: auto;

  콘텐츠 배경이미지 (height: 0px)  
  responsive-scale-bg {
    width: 100%;
    padding-bottom: 66.666666667%;
    background: url(img/fluid/image-1440x960.jpg);
    background-size: cover;
  }

  #### 재단 이미지
  컨테이너 요소의 폭에 맞쳐 크기가 동적으로 잘려지는 이미지를 말합니다.

  width: 100%;
  height: 960px;
  background-image: url(img/fluid/image-1440x960.jpg) center top;
  background-size: cover;


  #### 유연한 미디어
  유연한 아이프레임은 아이프레임을 포함하는 컨테이너 요소의 폭에 맞춰 크기가 변경되는 것을 말한다.

  비디오 같은 경우 width: 100% height: auto만 있어도 됩니다.

  ~~  {
    position: relative;
    padding-bottom: 56.25%;
    height:0;
    overflow: hidden;
    max-width: 100%
  }

  ~~ iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

</details>

<details id="17day">
  <summary>17일차</summary>
</details>

<details id="18day">
  <summary>18일차</summary>
</details>

<details id="19day">
  <summary>19일차</summary>
</details>

<details id="20day">
  <summary>20일차</summary>
</details>