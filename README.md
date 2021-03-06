# TIL
오늘 내가 배운 것들(Today I Learned)   

#### 4주차 질문

--------------------------------------------------

#### 4주 

| 일차                    | 링크                      |
| --------------------- | ----------------------- |
| 16일차                  | <a href="#16day">클릭</a> |
| 17일차                  | <a href="#17day">클릭</a> |
| 18일차                  | <a href="#18day">클릭</a> |
| <strong>19일차</strong> | <a href="#19day">클릭</a> |
| 20일차                  | <a href="#20day">클릭</a> |
---------------------------------------------------

#### 세번째 오프라인 강의
| 제목                           | 링크                      |
| ---------------------------- | ----------------------- |
| <strong>세번째 오프라인 강의</strong> | <a href="#3week">클릭</a> |


<details id="16day">
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

  #### 장치 독립적 픽셀 1

  환경이 변화되면서 장치마다 각각 픽셀을 어떻게 처리하는지 알아야하고 대응하는 방법이 무엇인지 알아야 합니다.
  https://brunch.co.kr/@blackindigo-red/18

  픽셀밀도 : 공간에 픽셀이 들어가는 물리적인 수치를 말한다. 
  멕칸토시는 처음에 인치를 사용해서 그 인치당 픽셀은 72픽셀이였다.

  디바이스 픽셀 밀도 : 애플사가 인치당 픽셀을 2배로 올려서 엄청나게 선명한 레티나 디스플레이를 소개한 이후, 디자인 과정에서 디바이스 픽셀을 고려해야한다.
  가로2배 세로 2배로 늘어남.

  벡터 그래픽 svg과는 달리 비트맵 그래픽은 픽셀 밀도에 영향을 받고, 고해상도를 지원하는 디바이스에 적합한 그래픽 제작이 필요하다.

  이롭게 라는 사이트. 메뉴는 선명하지만 로고는 선명하지 않다.

  css나 svg같은 경우 고해상도에 영향을 받지 않는다. 

  그래픽 디자인은 비트맵으로 작업을 많이합니다. 

  브라우저 개발툴 console => window.devicePixelRatio
  2 => 픽셀의 실제 이미지의 2배이기 때문에 사진의 이미지를 2배씩 올려야합니다.

  하지만 SVG로 만들게 되면 깨끗하게 보이게 됩니다.
  (이미지가 깨지면 SVG로 제작해야 됩니다.)

  네이버 같은 경우 네이버의 이미지는 깨져 보입니다. 하지만 애플 경우에는 이미지가 깨져보이지 않게 배율이 되면 2배의 이미지를 보여주게 됩니다.

  css에서 2배로 처리하면 되지 안냐? 스마트 오브젝트는 신기술 아니냐고 말하면 이렇게 말을 해야한다.  
  스마트 오브젝트를 이용해서 비율을 유지하고 크기를 올리세요. 스마트 오브젝트는 13년 전인 2005년에 나온 기술입니다. 안된다는 말 하지마시고 우선 해보시라고요.

  버튼으로 예를 들자면 1배수로 제작을 하고 2배수로 제작을 하는데 2배수로 제작을 하고 2분의1로 나누면 1배수가 됩니다. 하지만 디자이너는 이것을 고려하지 않고 89px같이 딱 나눠떨어지는 값을 사용하지 않아 브라우저가 이것을 픽셀로 만드는 데 문제가 생겨서 간격에 영향이 갑니다. 

  그럼 2배수로 하고 3배수로 하고 1배수로 만들려면 6으로 나눠서 떨어져야 하는데 이게 말이 됩니까?

  디자인을 2배수로하고 3배수로 하는 경우 이것은 실무 디자이너에 근본적인 설계 문제가 있다는 것입니다. 

  이 문제를 해결하는 방법은 시안을 1배수로 작업을 한다음에 픽셀 영향을 받는 이미지만 스마트 오브젝트를 이용해서 배율 이미지로 만들어서 받아야합니다.

  #### 장치 독립적 픽셀 2
  
  수치 측정 단위 중 픽셀 밀도를 측정하는 독립적인 단위가 없어 디자인 과정이 곤란 스러워졌다. 이에 대한 해결책은 애플은 Point(pt)를 제시했다. 

  더이상 px단위로 하지 않고 pt라는 단위를 제시했습니다.

  pt라는 것은 인쇄상에서 쓰이는 단위입니다. 같이 일하는 디자이너가 폰트 크기를 pt로 쓰는 디자이너가 있습니다. 정말 답답합니다.

  1x 1pt = 1px  
  2x 1pt = 2px

  모바일 애플리케이션 IOS 환경에서 장치독립적으로 변경되서 보여줍니다. 애플의 디자인은 PT라는 장치 독립적인 단위를 사용합니다. 하지만 웹은 아닙니다.

  그래서 안드로이드에서도 개발을 하였습니다. 그렇지만 PT라고 적게되면 애플을 배끼게 되는 것이라 안드로이드도 픽셀 밀도 DIP라고 하는데 이것을 DP라고 합니다. 하지만 애플과 다르게 안드로이드는 배율이 실수 단위입니다. 안드로이드는 열려있어서 많은 기업들이 가져다 쓰기때문에 혼돈이 왔습니다.

  디바이스 픽셀 밀도 UI 그래픽 내보내기. 픽셀 단위 그래픽이미지는 포토샵을 사용한다면 디자이너가 작업을 할때 벡터로 하는 게 좋겠지만 배율별로 이미지를 주는 게 좋다.

  그리고 1배수로 작업을 하자. 만약 벡터가 아닌 비트맵 이미지를 사용하지 않는 다면 스마트 오브젝트를 통해서 큰 이미지를 준비하세요. 애플 같은 경우 PT로 사용합니다. 

  사람이 보는 인식의 고려 
  1. 픽셀밀도를 낮추기.
  2. 버튼 크기를 바꾸기.

  고려해야할 것.
  1. 마우스 포인터와 손가락 크기는 다르다.
  2. 물리적인 크기.
  3. 사용자와 디바이스의 거리.

  대형 스크린 -> 픽셀 밀도 낮추기.

  가급적 이미지는 벡터로 그리고 디자인은 1배율로 작성합니다.

  웹은 운영체제보다 브라우저이기 때문에 보여주기가 중요합니다.

</details>

<details id="18day">
  <summary>18일차</summary>

#### 중단점과 미디어 쿼리 Lecture1

  [브레이크 포인트]
  RWD프로젝트 진행전, 주요 사용자 층이 사용하는 디바이스 환경을 분석한 후, 최적화되고 유효한 중단점(Breakpoint)을 설계(Design)를 한다.

  CSS3 미디어 쿼리 => 미디어쿼리는 각 디바이스 환경을 식별하는 조건 처리 구문으로 CSS3에서 정식 지원한다. 이를 사용하여 설계된 중단점에 맞는 최적화된 뷰 디자인을 구현할 수 있다.

  @media {type} and (expression) {...}  
  @는 사람들은 골뱅이라고 하는데 이것은 앳이라고 합니다.  
  [type] screen, printer, tv, integration css rule, projector를 넣을 수 있습니다.  
  [expression] and를 여러번 쓸 수 있습니다.  
  - 가로/세로 (width/height)
  - 풀컬러인지, 흑백인지 (color)
  - 화면비율 (aspect ratio) 
  - 독립적인 픽셀 단위 (resolution)
  - 가로형인지 세로형인지 (orientation)

```
width  : 가로 (min, max)
height : 세로 (min, max)
orientation : 회전 방향
aspect-radio : 회면 비율
color, color-index, monochrome  : 색깔
resolution : 독립적인 픽셀 단위 농도
```
- 디바이스 가로/세로 폭 길이 감지  
  /* width */  
  @media screen and (min-width: 600px) {...}  
  @media screen and (min-width: 200px) and (max-width: 400px) {...}  

  /* height */  
  @media screen and (max-height: 768px) {...}  
  @media (min-height: 500px) and (max-height: 580px) {...}  

- 디바이스 회전 방향 감지
  /* portrait */ 세로방향
  @media screen and (orientation: portrait) {...}

  /* landscape */ 가로방향
  @media screen and (orientation : landscape) {...}

- 디바이스 픽셀 밀도 감지
  /* 300 DPI */
  @media print and (min-resolution: 300dpi) {...}
  
  /* x2 Device  */
  @media screen and (min-resolution: 2ddpx)

- 논리 연산자 응용
  /* AND */ 모든 컬러를 사용하는 환경.
  @media all and (color) {...}

  /* NOT + AND */ 스크린만 아닌 것.
  @media not screen and (color) {...}

  /* ONLY + AND */ 
  @media only screen and (orientation: portrait) {...}

  /* COMMA */ 컴마도 가능
  @media all and (orientation: landscape),
         all and (min-width: 480px) {...}

#### 중단점과 미디어 쿼리 Lecture2

모바일 퍼스트 
현 시대 사용자 대부분이 모바일 환경에서 우선 접속합니다.
필요에 따라서는 데스크탑 환경이 필요(업무) 할 수 있습니다.
모바일 환경 디자인(설계)이 우선시 되어야 합니다.

중단점 설계

서비스를 이용하는 주 고객층의 행동 패턴을 분석하여
모바일, 태블릿, 데스크탑, 와이드 스크린 사용율 통계를 검토한 후,기기의 속성(스크린 폭, 해상도 등)을 고려하여 중단점을 설계해야 합니다.


중단점 설계를 위한 참고 자료

  - http://gs.statcounter.com
  - http://www.w3counter.com/globalstats.php?year=2018&month=3
  - http://www.internettrend.co.kr/trendForward.tsp
  - http://viewportsizes.com
  - http://troy.labs.daum.net
  - https://material.io/resizer

글로벌 서비스: 중단점 설계 (https://goo.gl/xQZwY6)

1.  360 x  640    23.4%
2. 1366 x  768   11.82%
3. 1920 x 1080    7.69%


대한민국 서비스: 중단점 설계 (https://goo.gl/dAQZG8)
  
 1. 1920 x 1080    22.90%
 2.  360 x  640    20.63%
 3.  375 x  667     7.54%


  디바이스(기기) 별 해상도
    
    [Mobile]
      Samsung Galaxy S9, S9+        :  360 x 740
      Samsung Galaxy S8, S8+, Note8 :  360 x 640
      iPhone 6(s), 7, 8             :  375 x 667
      iPhone X                      :  375 x 812

    [Tablet]
      iPad                          :  768 x 1024
      iPad Pro                      : 1024 x 1366
    
    [Desktop]
      Notebook                      : 1366 x  768
      Desktop                       : 1920 x 1080


  고려해야 할 중단점

    ⇐  (640) / 800  ⟺  (1024) / 1366  ⟺  1920  ⇒

    ※ 중단점은 최소한으로 설정할 필요가 있다.
      중단점이 많아지게 되면 기획/디자인/개발 
      과정이 모두 고통스러워지기 때문.


  고민해야 할 사용자 행동 패턴

    1920 스크린 해상도를 사용하는 사용자가
    풀 스크린으로 브라우저를 화면 가득 띄워놓고 사용하는지 확인 필요.
    그렇지 않다면 1366 기준으로 설계하되, 1920까지 고려하는 방향으로 전략 수립.
</details>

<details open id="19day">
  <summary>19일차</summary>
  
  #### WAI-ARIA 소개

  웹 콘텐츠 접근성 지침!

  WCAG 국제 웹표준 국제 기구  
  Web Content Accessibility Guidelines

  1997년 장애인들의 접근성 제고를 위해 WAI(Web Accessibility Initiative)를 설립하고 장애인이나 장애환경의 웹 접근성을 제고하기 위해 만든 가이드 라인입니다.

  WAI에서는 WCAG 1.0을 시작으로 2018년 6월 발표한 WCAG 2.1까지 웹 콘텐츠를 더 접근성 있게 만드는 권고안이 발표되었습니다. 

  지속적으로 업데이트 되고 있지만 웹접근성 수준을 보안 및 지원하기엔 빠르게 진화되는 신기술을 따라가기에는 아직도 많이 부족합니다.

  1. RIA의 동적인 웹 어플리케이션 접근성 보장을 위한 지침이 부족
  2. ajax를 통한 실시간으로 변경되는 컨텐츠를 못읽을 수 있습니다.
  3. 페이지 콘텐츠 중 일부만 변경시, 동일한 내용을 계속 읽어야 하는 문제 발생
  4. 화면 확대 사용자의 경우, 가시 범위 밖의 콘텐츠 변경 내용을 알 수 없음
  5. 기존 HTML 명세만으로는 웹 접근성 문제를 해결하기 어려움.

  접근성 권고안 발표 HTML5와 통합됨.

  WAL-ARIA는 스크린리더 및 보조기기 등에서 접근성 및 상호 운용성을 향상시키기 위해 마크업의 역활, 속성, 상태 정보를 추가할 수 있도록 지원합니다. 이렇게 마크업된 HTML은 각각의 운영체제의 접근성 API로 변환 되도록 설계되었습니다.

  운영체제 OS에서 제공하는 접근성 API를 통해 데스크탑 애플리케이션과 동일한 방법으로 자바스크립트 컨트롤을 인식하고 상호 작용 하게 됩니다.

  이것이 스크린리더 및 보조기기 사용자가 웹 애플리케이션을 사용할 때 데스크탑 애플리케이션 의 동작과 유사하게 인식하고 동작하기 때문에 보다 향상된 사용자 경험을 제공하게 됩니다.

  마크업에 역활, 속성, 상태 정보를 추가하여 스크린 리더 및 보조 기기 등에서 접근성 및 상호 운용성을 향상시키고보다 나은 사용자 경험을 제공하기 위함.

  #### WAI-ARIA 지원현황
  caniuse.com 라는 사이트에서 WAI-ARIA 라는 키워드를 검색해보면 모던 웹브라우저가 지원 수준이 상당히 높습니다. 그리고 스크린 리더 조사결과 JAWS와 인터넷 익스플로러의 조합의 호환성이 가장 높게 나타나고 있습니다.


  #### WAI-ARIA 속성(Properties)과 상태(States)
  WAI-ARIA를 소개하는 마지막 내용

  ARIA에서 등장한 3가지 기능

  ```HTML
  1. 속성(Properties)과 상태(States)
  속성과 상태는 요소가 기본적으로 가지고 있는 특징이나 상황
  속성과 상태 모두 aria라는 접두어를 가진다
  상태는 요소의 상황을 나타내는 정보로 애플리케이션이 실행되는 중에 자주 바뀌게 되지만 상태와 달리 속성은 바뀌는 경우가 드물다.

  ARIA의 속성 
  input 요소에 aria-required 속성의 값으로 true를 지정할 수 있습니다.
  스크린리더 사용자는 해당 입력 서식이 필수 항목임을 전달 받게 됩니다.
  <input type="checkbox" aria-required="true">

  추가적인 설명이 필요한 경우
   가령 입력서식에 입력값으로 영어 대소문자 및 특수문자와 숫자 등 3가지 유형의 조합으로 최소 10글자 이상 입력해야한다는 부가정보를 사용자에게 알리고자 할 때 추가 설명이 기재된 요소에 고유의 id를 지정 한 후 입력 서식에 aria-describedby 속성의 값으로 추가 설명이 기재된 요소의 id 값을 입력하는 것입니다.
   <input type="text" aria-describedby="reference">
   <div id="reference">추가설명</div>

   그룹 요소의 레이블을 정의할 때 입니다. 비단 그룹 레이블 뿐 아니라 다양한 요소의 레이블을 지정하는 용도로 사용할 수 있으며 긴 설명보다는 명사 등 간단한 이름으로 정의하여 해당 요소의 성격이 무엇인지 이해를 돕도록 할 수 있습니다.
   <div role="group" aria-label="레이블"></div>

   div 요소로 마크업 한 콘텐츠의 내용이 펼쳐진 상태인지 접혀진 상태인지 사용자가 알 수있도록 aria-expanded 속성을 사용했습니다. 이때 값으로 true를 지정하면 펼쳐진 상태를 의미하며 false가 지정되면 접혀진 상태 정보를 사용자에게 전달하게 됩니다.
   <div role="tabpanel" aria-expanded="true">

   입력 서식인 input 요소의 값이 유효한지 아닌지 오류 발생 상태 정보를 제공할 때 입니다. aria-invalid 속성을 사용할 수 있으며 true 의 경우 오류가 발생한 것을 의미합니다.
   <input type="text" aria-invalid="true">
  
  토글버튼의 상태 정보를 나타내기 위해 aria-pressed 속성을 사용할 수 있습니다. true의 경우 버튼이 눌러진 상태를 의미합니다.
  <button aria-pressed="true">
  ```

  #### WAI-ARIA HOW TO Use(1)

  ARIA를 사용할때 HTMl5 섹션 요소를 중복해서 사용하지 않는다.  
W3C 에서는 HTML5의 섹션 관련 요소와 WAI-ARIA 규칙을 함께 사용할 경우 해당 기능이 무효화 되거나 충돌이 발생할 수 있으므로 중복해서 사용하지 않도록 주의를 당부한다.

ARIA의 역할(role)과 비슷한 의미를 가진 HTML5 요소

role="application"은 동일한 역할의 HTML5 요소는 없음 주로 div 요소와 같이 그룹 역할을 하는 요소로 대체할 수 있다.

role="banner"은 동일한 역할의 요소 없음. 비슷한 의미로 header 요소를 사용할 수 있으나 로 사용할 경우 한 페이지에서 한 개의 요소만 사용하길 권장한다.

role="navigation"은 다른 페이지 또는 페이지 내 특정 영역으로 이동하는 링크 콘텐츠 영역을 의미하며 주로 메인 메뉴 및 서브 메뉴 등에 사용할 수 있다.

role="main"은 비슷한 역할의 요소로 main 요소가 있고 role="main"은 본문의 주요 콘텐츠 영역으로 한 페이지 내에 1개만 사용이 가능하며, 주의할 점은 role="main"을 article, aside, footer 요소의 하위 요소로 사용할 수 없다.

role="aside"은 비슷한 역할의 요소로 aside 요소가 있다. 주요 콘텐츠와 연관이 적은 의미있는 콘텐츠 영역으로 종종 사이드바로 표현할 수 있다. aside 영역에는 현재 날씨, 관련된 기사 또는 주식정보 등의 부가 콘텐츠를 포함할 수 있다.

role="form"은 비슷한 역할의 요소로 form 요소가 있으며 폼과 관련된 요소의 모임을 표현하는 영역으로 서버에 전송될 수 있는 콘텐츠를 포함 할 수 있다.

role="search"은 동일한 역할의 요소는 없다.

role="contentinfo"은 동일한 역할의 요소는 없으며 비슷한 의미로 footer 요소를 사용할 수 있으나 role="contentinfo"로 사용하였다면 한 페이지에서 한 개의 요소만 사용하길 권장합니다.

#### WAI-ARIA HOW TO Use(2)

HTML 요소의 네이티브(Native) 의미나 기능을 ARIA 규칙을 이용하여 변경하는 것은 바람직하지 않습니다.

h1 요소로 마크업하고 role=“button”으로 지정하는 경우 h1 태그안에 button을 넣거나 span 태그안에 role="button"을 넣어 주는 것이 중요합니다.

상호작용이 필요한 대화형 UI란 사용자가 클릭할 수 있는 정보나 탭 또는 드래그 앤 드롭, 슬라이드, 스크롤 등의 기능이 필요한 콘텐츠를 의미하는데 이런 대화형 UI를 div 요소나 span 요소 등으로 마크업하고 ARIA의 역할(role)을 통해 role=“button”으로 설정한 경우 사용자가 키보드로 해당 요소에 접근할 수 있도록 보장하는 것이 필요하다는 의미하다.

기본적으로 키보드 포커스를 받지 못하는 HTML 요소의 경우 키보드 포커스를 받을 수 있도록 하려면 tabindex 속성을 추가하여 문제를 해결할 수 있다.

숨긴 콘텐츠 
숨긴 콘텐츠에 특정 role을 부여했더라도 스크린 리더 등의 보조기기에서는 aria-hidden=“true”로 지정된 상태라면 의미적으로도 숨겨진 콘텐츠로 인식하게 됩니다.

```html
<button aria-hidden="true">버튼</button> X
<button aria-hidden="presentation">버튼</button> X

CSS의 display 속성에 none 값을 지정하여 스크린리더 등의 보조기기에서 접근할 수 없도록 하고 aria-hidden=“true”을 명시해야 합니다.
button {display: none;}
<button aria-hidden="true">버튼</button> o
```

모든 대화형 UI의 경우 반드시 레이블을 제공하여야 합니다. 레이블 제공을 위해 HTML의 label 요소를 사용하는 것을 권장하며 aria-label, aria-labelledby 등의 ARIA 관련 속성을 사용하여 레이블을 제공할 수도 있습니다.

```html
<div>
  <div id="user-name">이름</div>
  <input type="text" id="name" aria-labelledby="user-name">
</div>
```

#### WAI-ARIA 자동완성 UI

WAI-ARIA 를 적용하여 접근성을 개선한 사례
자동완성 ui

#### WAI-ARIA 데이터 검증결과
데이터 검증 예시에 사용된 WAI-ARIA 속성은 aria-live 이며 해당 속성을 통해 실시간으로 갱신 되는 정보를 스크린리더 사용자가 인지할 수 있도록 하였습니다.

#### WAI-ARIA 레이어팝업
 role="dialog"
</details>

<details id="20day">
  <summary>20일차</summary>
</details>

<details open id="3week">
  <summary>세번째 오프라인</summary>
  처음 시작할때 카카오에서 계좌 시스템을 개발하러 가셨을 때를 말씀해주셨다. 카카오 계좌시스템은 div로 되어있고 웹 접근성이 엉망이셨다고 하셨다.

  마크업한 것은 네비게이터 부분이였다. 
  Ul 요소 안에 li 요소를 넣고 그 부메뉴 부분을 ul요소를 써서 마크업을 했다.  

  ```html
  <ui>
    <li>
      <ul>
        <li>
          <a>
          ......
  ```

  그리고 웹 접근성을 위해 
  role="presentation"을 사용해 버튼이 스크린 리더가 인식되지 않게 하였다.
  그리고 눌렀을 때를 알려주기 위해 aria-haspopup을 사용했다. 왼쪽에 창이 열리기 때문에 aria-expended를 써준다.

  우리나라 사이트 중에서 웹 접근성에 민감하고 잘되어있는 사이트가 대한항공이 있다.

  대한항공은 웹 접근성이 잘 되어있지 않아서 해외로부터 소송을 당해 벌금을 냈다. 그래서 해외 시각장애인 단체를 찾아가 회의를 통해 개선하고 있다.

  네비게이션 부분을 마크업하게 되면 시간을 많이 사용 되기 때문에 네비게이터 부분을 복사해서 가져온다.

  그러면 네비게이터 부분에 버튼과 css 적용 안된 네비게이터가 보인다.

  버튼의 기본 속성 제거

  ```css
  .buttonNone{
    border: 0;
    background: transparent;
    padding: 0;
  }
  ```

  메뉴 버튼은 데스크탑일때 보이면 안된다.

  ```css
  /* 데스크탑 메인 메뉴 열기 버튼 */
  .buttonBurger{
    display: none;
  }
  ```

  그리고 버튼의 크기를 마춘 후에 appNavigation의 높이도 없애준다.
  ```css
  /* 모바일 내비게이션 */
  .appNavigation{
  }
  .buttonBurger{
    width: 40px;
    height: 40px;
    overflow: hidden;
  }
  ```

  햄버거 메뉴의 3개의 선들 추가
  
  ```css
  .burgerBar{
    display: block;
    width: 100%;
    height: 20%;
    background-color: #fff;
    position: absolute;
    left: 0;
    cursor: pointer;
  }
  ```

  햄버거 메뉴의 흰색 선들 위치 지정
  ```css
  .positionTop {
    top: 0;
  }
  .positionMiddle {
    top: 50%;
    transform: translateY(-50%);
  }
  .positionBottom {
    top: 100%;
    transform: translateY(-100%);
  }
  ```

  햄버거 메뉴 위치 수정
  ```css
  .buttonBurger{
    position: absolute;
    top: 60px;
    right: 20px;
    width: 40px;
    height: 40px;
    overflow: hidden;
  }
  ```

  버튼을 눌렀을떄 해당 버튼의 클래스에 isAct가 추가 되면서

  nav에 isAct가 추가 됩니다.

  그리고 버튼이 햄버거모양에서 x버튼이 되어야 합니다.

  맨위에 span태그가 45도로 꺽여야하니 rotate(45deg)로 꺾습니다.
  그리고 각도만 꺾으면 맨위에서 45도로 꺾이니 top을 50%만큼 줍니다.

  중간에 있는 스팬 태그는 위치를 유지한채로 왼쪽으로 이동하기 위해서 top: 50% 를 설정해주고 왼쪽으로 -105%만큼 보냅니다.

  그리고 맨 마지막에 있는 스팬도 가운데로 보내주고 -45deg를 줘서 반대반향으로 돌려줍니다.

  ```css
  .isAct .positionTop {
    top: 50%;
    transform: translateY(-50%) rotate(45deg);
  }
  .isAct .positionMiddle {
    transform: translate(-105%, -50%);
  }
  .isAct .positionBottom {
    top: 50%;
    transform: translateY(-50%) rotate(-45deg);
  }
  ```

  menu__list 라는 클래스를 넣어서 배경을 검은 색으로 배경을 넣은뒤에 X 버튼이 보이게 width를 70%을 준다.
  그리고 화면에 고정 시키기 위해 fixed를 주어서 height를 디바이스 크기에 마쳐서 100vh를 해야한다. 그리고 글자가 딱 붙어 있으면 이상하니 padding값을 설정한다.

  그리고 평소에는 안보이게 하기 위해 transform을 x쪽으로 -105%를 해준다. 버튼을 눌렀을 때는 보여줘야 하므로 transform을 초기화 시켜준다.
  
  ```css
  .menu__list {
    background-color: rgba(0, 0, 0, 0.85);
    color: #fff;
    width: 70%;
    height: 100vh;
    position: fixed;
    left: 0;
    top: 0;
    padding: 2em 1em;
    transform: translateX(-105%);
  }
  .isAct .menu__list {
    transform: none;
  }
  ```

  그리고 글자들이 붙어 있으니 글자들의 간격을 설정해준다.
  submenu 같은 경우 동적으로 나오는 것이라 !important를 설정해서 오차를 예방한ㄷ.
  a 태그는 인라인 태그라서 패딩값이 들어갈 수 있도록 block요소를 준다.

  ```css
  .menu__item {
    margin: 0.5em 0;
  }
  .menu__link {
    display: inline-block;
    padding: 1em;
    font-weight: 700;
    font-size: 1.6rem;
  }
  .menuAct .menu__subMenu{
    display: block !important;
  }
  .menu__subMenu li{
    margin: 0.5em 1em;
  }
  .menu__subMenu a{
    display: block;
    padding: 0.5em;
  }
  ```

  그 다음에는 li태그를 숨깁니다.

  모바일 작업이 전부 완료 되었으면 그다음은 데스크탑을 작업합니다.

  네비게이터의 색깔을 바까줍니다. 그리고 메뉴들을 가운데로 정렬하고 아이탬들은 float를 사용해서 왼쪽으로 배치 시킵니다.
  
  ```css
  /* 데스크탑 내비게이션 */
  .appNavigation {
    background-color: #988574;
  }
  .menu__list {
    width: 1000px;
    margin: 0 auto;
    color: #fff;
  }
  .menu__item {
    float: left;
    margin: 0 30px;
  }
  ```

  그리고 메뉴들의 크기와 간격을 설정합니다. 그리고 메뉴에 그림자를 주어서 더 선명하게 만듭니다.

  ```css
  .appNavigation {
    background-color: #988574;
    padding-top: 2em;
    padding-bottom: 1em;
  }
  .menu__list {
    width: 1000px;
    margin: 0 auto;
    color: #fff;
  }
  .menu__item {
    float: left;
    margin: 0 30px;
  }
  .menu__link {
    font-weight: 700;
    font-size: 1.6rem;
    cursor: default;
    text-shadow: 1px 1px 0 #000, -1px -1px 0 #000;
  }
  .menu__subMenu {
    padding-left: 1.5em;
  }
  .menu__subMenu li {
    margin: 0.5em 0;
  }
  .menu__subMenu a {
    display: block;
    padding: 0.5em;
  }
  ```
  
  그리고 폰텔로에 대해서 설명해주셨다. 폰텔로(fontello)는 아이콘을 선택해서 폰트처럼 사용할 수 있다고 한다. 
  기존에 있는 파일로 사용하기로 해서 index.css에 있는 소스를 넣어준다. 

  ```css

  ```
  그 다음에 자바스크립트 파일을 임포트 시켜줍니다.
  
  ```javascript
  <script src="./js/app.js"></script>
  ```

  

</details>

<details open id="3week">
  <summary>세번째 오프라인 후기</summary>
  오프라인 중에서 제일 쉬웠던 수업이였던 것 같다. 직접 해보라고 해서 어떻게 해야할지 몰랐는데 대충 감이 잡히는 것 같다. 야무님 프론트 강의에 반응형 웹디자인이라는 책이랑 오래가는 UX디자인이라는 것을 샀는 데 빠르게 복습하고 읽어야 겠다. 이렇게 따라치면 따라할 순 있을거 같은데 직접해보면 못따라갈 것같은 느낌이 든다.
</details>