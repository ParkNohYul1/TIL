# TIL
오늘 내가 배운 것들(Today I Learned)   

#### 1주차 질문

- ~~강의에서 서브라임 텍스트를 설치하라고 하셨는데. 클래스룸에서 VSCODE를 사용하라고 올라왔거든요.  오프라인 강의시둘다 사용하는 건지 아님 VSCODE만 사용하는 건지 궁금합니다.~~

- ~~```<br>```을 두번 사용하면 안된다고 하셨는데. margin으로 사용해서 빈칸을 주시는 건가 궁금합니다.~~

- ~~```<s>```요소를 취소선으로 사용 하셨는데. 제가 볼때는 전부 css로 처리 했었거든요. 영상보면 마크업이 재대로 안되어 있는 곳이 있다고 하셨는데. 혹시 ```<s>```나 text-decoration:line-through 둘중 어느 것을 많이 사용하시는지 궁금합니다.~~

- ~~유저 인터렉션 속성에서 나오는 tabIndex는 전부다 해주는 편인지 아니면 계획에서 나오는 대로면 해주는 편인지 궁금합니다.~~

- ~~문서 메타데이터 요소들에서 base라는 태그는 유용할 것같은데 실제로는 많이 사용을 안할 것같습니다. 혹시 이러한 태그를 요청 받거나 써줘야하는 상황이 있는지 궁금합니다.~~

- ~~달력 디자인을 받고 디자이너와 프론트를 디자인 했는데 css 경우 어떻게 관리를 해야 하는지 궁금합니다. 이미지를 따로 첨부하겠습니다.~~

- ~~우선 순위 경우 어떤 식으로 우선순위를 지정하는지에 대해 궁금합니다. 최대한 안겹치게 개발을 해야 하는지에 대해서~~

#### 2주차 질문
- 이번 주차는 동영상 보느라 바빠서 많이 질문을 준비하지 못했습니다. 10일차 학습 폼 스타일링에서 폼 컨트롤 가상 클래스는 IE 9+ 버전이하에서는 안먹히는데 만약 제가 저것을 사용하기 위해서는 제 위에 있는 PM이랑 상의하고 사용해야 되겠죠?


#### 오프라인 수업 질문
- 오늘 수업 들은 내용중에 important를 언제 쓰냐고 말씀해주신 것에 두가지가 있었는데 하나는 동적인 스타일이고 하나는 테스트 용도라고 하셨는데 동적인 스타일이 원리는 알았는데 정확히 어떤 것인지 파악을 못했습니다. 동적인 스타일이 어떤 경우인지 죄송하지만 한번더 말씀 부탁드려도 되겠습니까.

- 저희 프로젝트의 이미지를 미리 받아서 레이아웃을 나누는 실습을 해보는데 생각해보니 vh가 디바이스 높이라서 모바일에서 100vh만 주면 이미지가 잘려서  100vh 이상 줘야하는데 이번 시간은 flex에 대한 내용을 연습하기 위해서 하셨던 건지 아니면 flex로 계속해서 하시는 지 궁금합니다. 

---------------------------------------

#### 1주 

일차|링크
----|----
1일차|<a href="#1day">클릭</a>
2일차|<a href="#2day">클릭</a>
3일차|<a href="#3day">클릭</a>
4일차|<a href="#4day">클릭</a>
5일차|<a href="#5day">클릭</a>


#### 2주 

일차|링크
----|----
6일차|<a href="#6day">클릭</a>
7일차|<a href="#7day">클릭</a>
8일차|<a href="#8day">클릭</a>
9일차|<a href="#9day">클릭</a>
<strong>10일차</strong>|<a href="#10day">클릭</a>

#### 첫 오프라인 강의
제목 |링크
----|----
<strong>첫오프라인 강의</strong>|<a href="#1week">클릭</a>

## 구조 디자인(HTML) 
<details id="1day">
  <summary>1일차 학습</summary>
  

#### [HTML 이란?]
  - HTML이란 링크 형식의 시스템입니다.  
  - MarkUp은 구조입니다.   
  - Language는 언어입니다.  
  - 구조를 설계할때 사용 하는 언어  
  - HTML은 텍스트 파일인데 웹 브라우저가 구조를 화면에 표현하기 위해 랜더링을 합니다.

<br>
  
#### [시멘틱 마크업]
  - 웹브라우저가 자동으로 우리가 만들지 않았던 것을 구성하는데 이것을 마크업이라고 합니다. 
  HTML은 시작이 있으면 끝으로 감싸줘야합니다.
  - heading 요소는 웹 표준이라는 규칙에 맞게 ```<H1>``` 으로 작성해야 하고
  paragraph 요소는 ```<P>```로 작성해야 합니다.

<br>
  
#### [기본 문법]
  - HTML은 헤드영역과 바디영역으로 구성되어 있습니다.  

  HTML 용어  


용어|설명
----|----
element|요소
open tag|여는 태그
close tag|닫는 태그
attribute|속성
value|값


  기본문법<br>

  ```
  <태그이름 속성="값"> 컨텐츠 </태그이름>
  ```

  ```
  <tag attr="value"> 개발도구(DevTools) </tag>
  ```

  - title 속성은 tooltip 이라고 하는데 말풍선이라고도 볼 수 있습니다.
  - 문서를 작성하면 웹 브라우저가 해석해서 유저 인터페이스를 처리해줍니다.
  - 사용자가 보는 것은 body 그리고 브라우저에게 정보를 제공하는 것을 head라고 합니다.
  - ```<html>```태그는 해당 파일의 뿌리가 되므로 root element라고 합니다.

  ```
  인코딩 확인하는 방법 : 콘솔창에 document.characterSet 입력 
  ```
<br>

#### [텅 빈 요소]
  - empty Elements 컨텐츠를 감싸지 않는 요소입니다.
    ```html
    닫는 태그가 없는 이유는 감싸줄 것이 없기 때문입니다.
    <meta charset = "utf-8">
    ```

<br>

#### [표준 호환모드]
  - HTML과 HEAD사이와 BODY와 HTMl 사이에 그리고 HEAD와 BODY 사이에는 어떤 것도 들어가면 안됩니다.
  - 들여쓰기 INDENTATION 사람이 보기 편하게 하기 위해 사용합니다.
  - 태그는 대문자와 소문자로 쓸 수 있지만 웬만하면 소문자로 작성해야 합니다.
    ```
    표준 모드와 비표준 모드 확인 방법 : 콘솔 창에 document.doctype 입력
    ```

<br>

#### [주 언어 설정]
  - 문서에 사용되는 주 언어 설정

  언어|코드
  ----|----
  한국어|ko
  영어|en
  일본어|ja
  스페인어|es

  - 화면을 읽는 스크린 리더를 사용하기 위해 사용합니다.

    ```html
    <html lang="Ko-KR">
    ```

<br>

#### [제목과 단락]

  사용자가 가장 많이 읽는 콘텐츠는 단락(Pararaph)입니다. 단락은 ```<p>```요소로 구성됩니다.

  ```html
  <p>사용자가 가장 많이 읽는 콘텐츠는 단락(Paragraph)입니다.</p>
  ```

  - 사용자가 가장 먼저 읽는 콘텐츠는 제목(Headings Level 1~6)입니다. 제목은 ```<h>```요소로 구성됩니다.
  - h1 태그는 문서에서 하나만 작성해야 한다.
    ```html
    <h1> 제목 1</h1>
    <h2> 제목 2</h2>
    <h3> 제목 3</h3>
    <h4> 제목 4</h4>
    <h5> 제목 5</h5>
    <h6> 제목 6</h6>
    ```

  - HTML 주석은 브라우저에서 해석되지 않습니다.

    ```html
    <!-- HTML 주석 코드는 브라우저에서 해석되지 않습니다. -->
    ```

<br>

#### [이미지와 피규어]
  - HTML 문서에 연결되어 화면에 표시되는 이미지 요소와 도표, 차트, 표, 이미지 등을 캡션과 함께 묶어주는 피규어 요소에 대해 공부합니다.


    ```
    웹 문서에 주로 사용 되는 이미지 포맷 : JPG, GIF, PNG, SVG
    ```

    - JPG
    ```
    JPG 이미지는 압축률이 높고 다양한 색상을 처리하도록 설계되었습니다.   
    사진 또는 복잡한 그래픽(그레디언트와 같은) 이미지에 많이 사용 되는 포멧입니다.  
    ```
    - PNG
    ```
    PNG 이미지는 사진이나 애니메이션을 제외한 모든 유형에 적합합니다.   
    사진의 경우 동일한 품질의 PNG 파일 크기가 일반적으로 JPG보다 크기 때문입니다.  
    하지만 JPG와 달리 투명 처리가 가능해 아이콘, 로고, 다이어그램 등에 사용하면 좋습니다.
    ```

    - GIF
    ```
    GIF 이미지는 표현 가능한 색상이 256색으로 제한되어 있기에 사진에는 적합하지 않습니다.   
    하지만 애니메이션을 적용할 수 있는 포멧으로 단순한 그래픽의 애니메이션에 사용하면 좋습니다.   
    투명하게 처리가 가능하긴 하지만, PNG 포멧 보다 표현력이 떨어집니다.
    ```

    - SVG
    ```
    SVG 이미지는 벡터 기반 그래픽 포멧으로 품질 손실없이 확대, 축소 할 수 있습니다.    
    오늘날 처럼 다양한 스크린에 대응하는 반응형 웹 디자인에 매우 적합합니다.    
    왼쪽 이미지인 SVG와 달리 오른쪽 이미지인 비트맵 이미지는 크기를 키울 경우 뿌옇게 표시됩니다.    
    픽셀로 구성된 그래픽    
    ```

  - img의 src는 source를 줄인말이다. alt는 alterate text를 줄인 말이다.
  - figure, figcation
    ```html
    <figure>
      <img
        src="sbs-drama__do-you-want-to-kiss-first.png"
        alt="SBS 드라마 <키스 먼저 할까요?>의 한장면: 배우 김선아가 홀로 겨울바다를 걷는 중...">
      <!-- figure cation -->
      <figcation>
        - 이미지 출처: SBS <키스 먼저 할까요?> 방송화면 캡쳐-
      </figcation>
    </figure>
    ```




#### [문법 검사]
  ```
  문법 검사 사이트 : validator.w3.org
  엔티디 코드 사이트 : entitycode.com
  ```

<br>

#### [순차/비순차 목록]
  - ```<li>``` list item 목록 아이탬
  - ```<ul>``` unordered List 비순차 목록 * bullet 총알 모양처럼 생겨서 bullet이라고 함
  - ```<ol>``` ordered List 비순차 목록

  ```html
  <ul>
    <li>그녀들의 컬쳐 라이프</li>
    <li>언니들의 핫 플레이스</li>
    <li>스타, 그옷 어디꺼?</li>
    <li>화장품 리얼 리뷰 기초편</li>
    <li>화보 속 스타</li>
    <li>패션 가이드북 의류편</li>
  </ul>
  ```

  ```html
  <ol>
    <li>62세에 미니스커트 완벽 소화한 비결</li>
    <li>놀라운 패션센스, 사우디 공주의 우아한 일상</li>
    <li>고양이 자세를 매일 해야 하는 이유 5가지</li>
    <li>여자컬링 '안경 선배'가 쓴 안경은 대구산 '플럼'</li>
    <li>이게 유행이라고?</li>
  </ol>
  ```

<br>

</details>

---------------------------------------

<details id="2day">
  <summary>2일차 학습</summary>
  

#### [앵커와 하이퍼링크]
  - A 태그 ANCHOR

    ``` html
    a 요소에 href 속성을 사용하여 링크 주소를 설정합니다. 문서가 길때 해당 페이지의 원하는 지점으로 점핑을 합니다.
    <a href="#">HELLO</a>
    ```

    ```html
    해당 아이디를 가진 요소로 이동하는 태그
    <h2>목차(Table of Contents)</h2>

    <ul>
      <li><h3 id="#intro">소개</h3></li>
      <li>
        <ul>
          <li><a href="#">영상 소개</a></li>
          <li><a href="#">어렵지 않을까 걱정되시나요?</a></li>
          <li><a href="#">GSAP에 대해 간략하게 정리해볼까요?</a></li>
          <li><a href="#">TweenLite</a></li>
          <li><a href="#">TimelineLite</a></li>
          <li><a href="#">TimelineMax</a></li>
          <li><a href="#">TweenMax</a></li>
          <li><a href="#">기타 도구</a></li>
          <li><a href="#">다운로드 & CDN</a></li>
        <ul>
      </li>
    </ul>
    ```

    ```html
    <h2>인기기획전</h2>

    <ul>
      <li>
        <a href="http://shopping.daum.net/event/detail/31889">
          인어공주인 줄 알았어, 바디라인이 돋보이는 레이스 스커트
        </a>
      </li>
      <li>
        <a href="http://shopping.daum.net/event/detail/31857">
          휴대폰에 체크를 입혔어, 키링으로 예쁨을 더해준 케이스
        </a>
      </li>
      <li>
        <a href="http://shopping.daum.net/event/detail/31856">
          흑채 스프레이면 10년은 젊어 보여, 풍성한 헤어 연출해요
        </a>
      </li>
      <li>
        <a href="http://shopping.daum.net/top">
          우리 아이 어린이집 첫 등원! 당일 배송으로 준비물 챙겨요
        </a>
      </li>
      <li>
        <a href="http://shopping.daum.net/event/top">
          기획전
        </a>
      </li>
      <li>
        <a href="http://shopping.daum.net/bestshop/soho.daum?menuyn=y">
          소호 BEST
        </a>
      </li>
    <ul>
    ```


  - 절대 경로
  
    ```
    현재 HTML 문서와 상관없이 URL 주소를 사용하여 리소스를 찾는 것을 말합니다.
    http://domain.com/resource.html
    ```

  - 상대 경로

    ```
     현재 HTML 문서에서 상대적인 위치를 설정하는 것을 말합니다.
     ../misc/extras.html
    ```

  - 루트 경로

    ```
    현재 HTML 문서가 존재하는 영역의 최상위 루트 경로에서 대상을 찾는 것을 말합니다.
     /images.html
    ```

<br>

#### [설명 목록]
  - DL 설명목록

    ```
   <dl> 설명 목록(Description Lists) </dl>
    ```

  - DT 용어

    ```
    <dt> 용어(Definition Term) </dt>
    ```  
  - DD 설명

    ```
    <dd> 설명(Definition Desciption) </dd> 
    ```

    - 사용법

      ```html
      <h2>추가 정보조회</h2>

      <dl>
        <dt>워런티</dt>
        <dd>
          <img src="images/additional-info-icon-warranty-mo.png" 
          alt="warranty" title="warranty" width="48" height="48">
          <p>제품 등록 후 보증 정보를 확인하세요.</p>
          더 보기
        </dd>

        <dt>윈도우 업데이트 정보</dt>
        <dd>
          <img src="images/additional-info-icon-window-mo.png"
           alt="Windows update information" title="Windows update information" width="48" height="48">
          <ul>
            <li> Windows 10 업데이트 안내</li>
            <li>Windows 10 S 지원 모델 정보</li>
          </ul>
        </dd>

        <dt>Samsung Flow</dt>
        <dd>
          <img src="images/Home_addinfo_SamsungFlow.png" 
          alt="samsung flow" title="samsung flow" width="48" height="48">
          <p>PC 로그인, 모바일 핫스팟 연결 및 모바일 알림 동기화 기능을 간편하게 사용하실 수 있습니다.</p>
          <a href="">더 보기</a>
        </dd>

        <dt>뉴스 & 공지사항</dt>
        <dd>
          <img src="images/additional-info-icon-alert-mo.png" 
          alt="news & notification" title="news & notification" width="48" height="48">
          <p>제품 및 서비스에 대한 공지사항</p>
          <a href="">더 보기</a>
        </dd>
      </dl>
      ```

    - IMAGE ALT속성은 스크린 리더를 이용하여 장애우분들이 들을 수 있도록 해줍니다. 일반 사용자가 보려면 TITLE을 사용해야합니다.
    - 아이콘은 동일한 크기로 만들기 위해 인스펙트 요소로 마우스를 올려서 크기를 확인한 다음에 동일한 크기로 마쳐줍니다.

<br>


#### [인용과 줄 바꿈]

  - 인용문
    
      ```
      HTML Quote 요소 (<q>)는 둘러싼 텍스트가 짧은 인라인 인용문이라는 것을 나타냅니다. 이 요소는 단락 구분이 필요없는 
      짧은 인용문을 위해 사용되며, 긴 인용문에는 <blockquote> 요소를 사용하세요.
      ```
  
  - 출처를 표기하기 위해 사용, 제목을 반드시 포함
    ```html
    <blockquote>
        <p>It was a bright cold day in April, and the clocks were striking thirteen.</p>
        <footer>
            First sentence in <cite><a href="http://www.george-orwell.org/1984/0.html">Nineteen Eighty-Four</a>
            </cite> by George Orwell (Part 1, Chapter 1).
        </footer>
    </blockquote>
    ```

  - q 인용 태그는 중첩이 가능합니다. 꼭 q를 사용할 필요없이 ```'```를 사용 할 수 있고, 단어 강조는 q요소가 적합하지 않습니다.
    ```html
    어렸을 때 어른들이 <q>너 많이 컸구나</q> 하면 그게 굉장한 칭찬으로 느껴졌었습니다. 다만 시간이 지난 것뿐인데…
    지금은 <q>너 아직도 노안이 안 왔구나</q> <q>너 아직 머리숱이 많구나 (혹은 너 아직도 흰머리가 덜 났구나)</q> 등의 
    이야기가 퍽 반갑습니다. 어렸을 때는 시간이 흐른 것 때문에 칭찬받고, 나이 들어서는 시간을 비껴간 것 때문에 칭찬 비슷
    한 것을 듣습니다.

    나이가 들었다는 걸 깨닫는 건 흰머리가 늘었다는 사실을 발견하는 순간이 아닙니다. 그 흰머리를 대수롭지 않게 여기고 
    있다는 걸 발견하는 순간이지요. 듬성듬성 해진 머리, 오르기 시작한 뱃살, 거칠어져가는 피부, 예전 같지 않은 체력, 
    불쑥 찾아 드는 허무감… 나이 듦의 징후는 몸도 몸이지만 무엇보다 급격히 줄어든 자신감, 즉 심리적 위축감에서 확연히 
    드러납니다.
    ```

    - 출처는 city 요소를 사용.
    ```html
    <figure>
      <img src="images/sbs-drama__do-you-want-to-kiss-first.png" alt="">
      <figcaption>-이미지 출처: SBS &lt; 키스 먼저 할까요? &gt; 방송화면 캡쳐-</figcaption>
    </figure>

    <blockquote>
      <p> "...우리 같은 여자들은." </p>
      <p> "우리" </p>
      <p> "아 너무 말 많다 말 짧게 하자 우리 쓰기 귀찬다" </p>
      <p> "ㅇㅋ" </p>
      <cite>_SBS 드라마 <키스 먼저 할까요?> 중에서</cite>
    </blockquote>
    ```

    - LINE BREAK ```<BR>``` 줄바꿈(개행) ```<br>``` 요소는 2번 사용 하면 안됩니다.
    ```
      맞아요. 안 늙었어요, 나는 아직.<br>
      그렇게 안 봐주는 세상 때문에 매 순간 늙고 있어서 그렇지.
    ```

<br>

#### [어휘 요소들]
  - 강조하는 것은 의미가 있고 표현 하는 것은 의미가 없습니다.
  - 구조 디자인은 쉽지 않고 내용을 이해하고 구조화를 해야 됩니다.


  ```html
    <strong>, <em>, <b>, <i>
  ```

  - 시멘틱 요소 (의미 요소)
    - ```<strong>``` : 내용의 중요성, 심각성, 긴급성을 강조할 경우 사용
    
      ```
        [중요성] : 제목/캡션의 글자 중 일부를 더욱 강조하는 데 사용
        [심각성] : 경고 또는 주의를 주고자 할 때 사용
        [긴급성] : 문서의 다른 부분보다 빨리 보아야 하는 내용을 나타내는데 사용
      ```

    - ```<em>``` : 특정 내용의 스트레스 강조 - 문장 의미를 변경
      ```html
      강조가 없는 예 
      <p>고양이는 귀여운 동물입니다.</p>

      고양이<종>을 강조한 예
      <p><em>고양이</em>는 귀여운 동물입니다.</p>

      귀여운(형용사)를 강조한 예
      <p>고양이는 <em>귀여운</em> 동물입니다.</p>

      동물을 강조한 예
      <p>고양이는 귀여운 <em>동물</em>입니다.</p>

      문장 전체를 강조한 예 (느낌표 사용)
      <p><em>고양이는 귀여운 동물입니다!</em></p>
      ```

  - 넌 시맨틱 요소 (의미가 없는 요소) 다른 글자와 구분하기 위한 용도
    - HTML5에서는 ```<b><i>```요소를 다른 형태로 사용 할 것을 권장

    - ```<b>``` : 단순히 다른 글자와 구분된 용도로 사용 문서 요약의 주요단어, 리뷰 제품 이름 등

      ```
        작은 방에 들어가니 <b>낡은 액자</b>와 <b>거미줄이 엮인 손전등</b>이 탁자에 놓여있었다.
      ```

    - ```<i>``` : 다른 글자와 구분된 용도로 사용. 기술적 용어, 다른언어(목소리), 인물의 생각 등을 표현

      ```html
      <p><i class="taxonmy">펠리스 실베스트리 카터스(Felis silvestris catus)</i>는 귀여워요. <p>
      <p>
      ~는 재판을 받고 나오면서 
      <i lang="la">"E pur si muove."</i>
      라고 말했습니다.
      </p>
      ```

    - 제목은 ```h1``` ```h6```요소를 사용하고 강조는 em 요소를 사용해며, 중요도는 strong 요소로 표시 되어야 하고, 표시 또는 강조 표시된 텍스트는 mark 요소를 사용합니다.

<br>


#### [섹션/메인 요소]
 - 루트 섹션(Root Section) 요소
  ```
  <body>
  문서에서 단 1번만 사용 가능
  ```
[섹션(Sections) 요소들]
  ```
  섹션 요소는 일반적인 컨테이너 요소가 아니며, 문서 개요에 명시적으로 나열되는 경우에만 섹션 요소가 적합하다는 규칙이 있
  다. 일반적인 컨테이너 요소로는 <div><span>이 있다.
  ```
 - ```<article>```
  ```
 문서, 페이지, 애플리케이션, 사이트 등에 포함된 독립적인 세션을 말한다. 
 잡지, 신문, 논문, 에세이, 보고서, 블로그, 기타 소셜 미디어 일 수 있음
 일반적인 규칙은 article 요소는 일반적으로 요소의 하위 항목으로 제목(h1~h6 요소)를 포함시켜 식별해야 한다. 
 제목 없이 컨테이너 요소로 사용하면 안되고 반드시 제목을 포함시켜야 한다.
  ```
 - ```<section>```
  ```
  문서, 어플리케이션의 일반적인 섹션을 말한다. 이 컨텍스트의 섹션은 그룹화 된 콘텐츠이다.
  웹 사이트의 섹션은 소개(introduction), 뉴스 항목(new item), 연락처 정보 (contact information)를 위한 
  섹션으로 나눌 수 있다.

  [참고] 콘텐츠 요소가 포함된 독립적인 섹션의 성향이 크다면
  section 요소 대신 article요소를 사용하는 것이 좋다.
  ```
 - ```<aside>```
  ```
  웹 사이트의 사이드바에 해당되는 부 콘텐츠(메인 콘텐츠와 분리된) 섹션을  말한다. (메인과 관련이 없고 광고같은 부분)
  ```
 - ```<nav>```
  ```
  다른 페이지로 이동하는 링크 또는 사이트 내 검색 링크를 포함하는 섹션 요소이다.

  [참고]
  내용을 쉽게 이해할 수 있도록 nav 요소 내부에는 비순차목록 (ul)을 사용한다. 사이트의 모든 링크를 nav에 포함하는 것은 
  아니며, 주로 사이트를 탐색하는 링크를 포함한다. 사이트 하단에 위치랑 링크는 footer요소로도 충분하다.
  ```
 - ```<header>```
  ```
  header 요소는 일반적으로 세션의 제목, 목차, 검색, 로고 등을 포함하는데 사용한다.
  ```
 - ```<footer>```
  ```
  footer 요소는 일반적으로 섹션의 저자, 링크, 저작권 정보 등을 포함하는데 사용한다.
  ```
 - ```세션과 헤딩```
  ```
  헤딩(h1 ~ h6) 요소는 세션의 제목에 해당된다.
  ```

 - ```<main>``` 메인 (Main) 요소
  ```
  문서 또는 애플리케이션 body 요소의 메인 콘텐츠에 해당 한다.
  main 요소는 섹션 요소가 아니며, 보이는 요소가 2개 이상이면 안된다.
  사용하지 않는 다면 숨김 처리를 해야한다.
  article, section, aside, nav요소는 main요소를 자식으로 포함할 수 없다.
  반대로 main은 가능하다. main 내부에는 header, footer 요소를 직접적으로 포함하지 않는다.
  ```

  실습 
  ```html
  <header>
    <h1><a href="/">JTBC</h1>
    <nav id="global0navigation">
      <h2>글로벌 내비게이션</h2>
      <!-- ... -->
    </nav>
    <aside id="review-banner">
      <h3>리뷰배너</h3>
      <!-- ... -->
    </aside>
  </header>

  <main>
    <article id="on-air-banner">
      <h2>온에어 배너</h2>
      <!-- ... -->
    </article>
    <section id="realtime-vod">
      <header>
        <h2>리얼타임 VOD</h2>
      </header>
      <!-- ... -->
    </section>
    <article id="daily-programs">
      <h2>데일리 프로그램 소개</h2>
      <!-- ... -->
    </article>
    ~~
    ~~
  </main>
  <footer>
    <nav id="footer-navigation">
      <h3>푸터 네비게이션</h3> 세션제목
      ...
  </footer>
  ```

  ** 세션은 무조건 헤딩 요소가 필요합니다.
</details>

---------------------------------------

<details id="3day">
  <summary>3일차 학습</summary>
  
#### [컨테이너 요소]

 - HTML 요소를 묶는 컨테이너 요소들
 ```
  아무런 의미(Semantic)는 가지지 않는다.
  그러하므로 이 요소들은 적절한 시멘틱 요소가 없을 때 사용해야한다.
 ```
 - ```<div>``` 디비전 (Division) 요소
  ```html
   - 블록(block) 컨테이너

   <style>
      .division {border: 1px solid #505050;}
   </style>

   <article lang="en-US">
      <h2>My use of language and my cats</h2>
      <p>My cat’s behavior hasn’t changed much since her absence, except
      that she plays her new physique to the neighbors regularly, in an
      attempt to get pets.</p>
      <div lang="en-GB" class="division">
        <p>My other cat, colored black and white, is a sweetie. He followed
        us to the pool today, walking down the pavement with us. Yesterday
        he apparently visited our neighbours. I wonder if he recognizes that
        their flat is a mirror image of ours.</p>
        <p>Hm, I just noticed that in the last paragraph I used British
        English. But I’m supposed to write in American English. So I
        shouldn’t say "pavement" or "flat" or "color"...</p>
      </div>
      <p>I should say "sidewalk" and "apartment" and "color"!</p>
    </article>


  ```

 - ```<span> 스펜(Span) 요소```
  ```html
  인라인(inline) 컨테이너
  인라인 요소들(a, strong, em, b, i 등)을 감쌀 때 사용된다.
  블록 요소들(h1~6, p, blockquote, section 등)을 감쌀 수 없다.

  <style>
    .division {border: 1px solid #505050;}

    .green  { color: #71c456; }
    .yellow { color: #fec417; }
    .orange { color: #fc9500; }
    .red    { color: #e9524d; }
    .violet { color: #a953ac; }
    .blue   { color: #13ade6; }
  </style>

  <h2>
      SIX
      <span class="green">C</span>
      <span class="yellow">O</span>
      <span class="orange">L</span>
      <span class="red">O</span>
      <span class="violet">R</span>
      <span class="blue">S</span>
    </h2>
  ```

<br>


#### [텍스트 레벨 요소]
 - 아래 첨자 (sub script text) ```<sub>```
  ```
  기준선의 아래, 다른 글자의 오른쪽에 놓이는 작은 글자, 대부분 화학식이나 수학식에 사용된다.
  ```
 
 - 위첨자 (super script text) ```<sup>```
  ```
  다른 글자의 오른쪽 위에 놓이는 작은 글자. 때떄로 약어에서, 그리고 각주를 나타낼 때도 사용된다.
  ```

 - 하이라이트 ```<mark>```
  ```
  관련 참조 목적의 하이라이트된 글자 요소
  ```

 - 축약 ABBREBIATION  ```<abbr>``` 요소

 - 타임 요소 ```<time>```
  ```
  기계가 이해할 수 있는 형태로 날짜나 시간을 나타내는 요소
  ```

 - 취소 요소 strikeThrough ```<s>```
  ```
  더 이상 관련이 없거나 더 이상 정확하지 않은 요소
  ```

  - 정의 요소 ```<dfn>```

  실습 
```html
<!-- sub, sup -->
<h2>아래첨자</h2>
<p>
  기준선의 아래, 다른 글자의 오른쪽에 놓이는 작은 글자. 대부분 화학식이나 수학식에 사용된다.
</p>
<dfn id="sulfuric-acid">
  H<sub>2</sub>SO<sub>4</sub>
</dfn>

<blockquote cite="https://ko.wikipedia.org/wiki/%ED%99%A9%EC%82%B0">
  <p>
    황산은 강산성의 액체 화합물이다. 중국과 일본에서는 유황의 산이라 하여 硫酸이라고 하며, 북한에서도 류산이라고 한다.
    우리나라에서도 유산이라는 말을 쓰기도 하지만 젖산을 뜻하는 유산과 착각할 수 있으므로 황산을 사용한다.
    물을 제외하고는 가장 많이 제조되며, 많은 곳에 사용된다. 2001년의 세계 황산 생산량은 1억 65백만 톤에 달한다. 
    비료 제조, 광석 처리, 폐수 처리, 석유 정제 등에 사용된다.
  </p>
  <cite>위키백과에서</cite>
</blockquote>

<h2>윗첨자</h2>
<p>
  다른 글자의 오른쪽 위에 놓이는 작은 글자. 때때로 약어에서,
  그리고 각주<sup><a href="#footnote-1">[1]</a></sup>를 나타낼 때도 사용된다.
</p>

<!-- mark, time -->
<article>
<h3>2장. - 최적의 각도를 찾아라</h3>
<img src="images/pyramid.png" alt="피라미드(최적의 각도를 찾아라)">
<p>
  내용은 다음과 같습니다. -고대 이집트인들은 시키드(seked)라는 특별한 각도를 사용했다. 
  -시키드는 현대 삼각함수의 코탄젠트(cotangent)와 그 값이 같다. 
  <mark>삼각함수</mark>와 코탄젠트라는 단어에 멈칫했을 수도 있지만, 이것을...
</p>
<span class="article-share">공유 <data value="0">0</data></span> &middot; 
<span class="article-comments">댓글 <data value="0">0</data></span> &middot;
<cite><time datetime="2018-02-22"> Feb 22. 2018</time> by sortie</cite>
</article>

<!-- abbr, time -->
<article class="news-item">
  <h2>일본만 팔던 <abbr title="맥도날드">맥날</abbr> 초콜릿 파이.. 오늘부터 한국서 판매</h2>

  <p>
    뉴스팀 입력 <time datetime="2017-08-14T10:18">2017.08.14 10:18<time>
    <span class="article-comments">댓글 <data value="0">0개</data></span>
  </p>
  <img src="images/macdonald.jpg" alt="맥도날드 초콜릿 파이">
  <!-- ... -->
</article>


<!-- s, time -->
<ul>
  <li>
    <img src="images/cable-holder.jpg" alt="">
    <h3>
      <span class="sub-headline">마그네틱 자석 선정리 케이블홀더</span>
      [슈퍼특가] 자석식 선정리기 케이블 홀더
    </h3>
    <p>
      <span class="hidden-text">원래가격</span><s>11,900원</s>
      <em>50%<em> <span class="hidden-text">할인</span> 5,900원
    </p>
  </li>
  오늘마감 7개 구매
<ul>

<!-- 수평선: horizontal rule -->
<hr>

<!-- 각주: footnote -->
<div>
  <p>
    <a id="footnote-1" href="#footnote-o-1">[1]</a> 각주(脚註, 영어: note)는 본문에 대한 참조 문헌이나 
    본문의 낱말, 문장 등의 뜻을 알기 쉽게 풀이하는 덧붙이는 글이다.
  </p>
</div>
```

<br>


#### [그룹핑 요소]

  ```html
    <main> 요소
    <div> 요소
    <blockquote> 요소
    <p> 요소
    <ul> 요소
    <ol> 요소
    <li> 요소
    <dl> 요소
    <dt> 요소
    <dd> 요소
    <figure> 요소
    <figcaption> 요소
    <hr> 요소
    <address> 요소
    <pre> 요소

  ```

  - address 사람들과 조직의 정보를 나타낼 때 사용합니다.

  - small 저작권
  
  - 전화번호 인 경우 href tel로 연결 해야 합니다.

  - 사업자 번호에도 사업자 정보를 볼 수 있는 링크를 걸어줍니다.

    ```html
    <address>
      <p>W3C on Twitter</p>
      <p><a href="https://twitter.com/w3c">w3c</a></p>
    </address>
    ```

  - pre 코드의 줄바꿈 여백을 그대로 유지 합니다.

    ```html
    <pre>
      function fnSetMenu(vGbn) {
        $('.br-menu-link').each(function(idx){
          if ( $(this).attr('href') != '#none' ) {
            var vHref = $(this).attr('href');
            var menuId = vHref.substring(vHref.indexOf('menuId='), vHref.length);
            vHref = vHref.substring(0, vHref.indexOf('isMain=Y'));
            $(this).attr('href', vHref + 'isMain=Y&gbn=' + vGbn+"&"+menuId);
          }
        });
        
        $('.sub-link').each(function(idx){
          var vHref = $(this).attr('href');
          var menuId = vHref.substring(vHref.indexOf('menuId='), vHref.length);
          vHref = vHref.substring(0, vHref.indexOf('isMain=Y'));
          $(this).attr('href', vHref + 'isMain=Y&gbn=' + vGbn+"&"+menuId);
        });
      }
    </pre>
    ```

  - pre 코드는 앞 공백까지 인식하기 때문에 붙여야 합니다.

  실습 

  ```html
  <address>
    <!-- address -->
    서울특별시 강남구 삼성로 648 SM ENTERTAINMENT
    Communication Center 대표전화 <a href="tel:+82262409800">02 6240 9800</a>
    <!-- 사업자 등록조회 확인: https://goo.gl/XqFuCC -->
    대표 : 한세민, 남소영 사업자번호 <a href="https://goo.gl/xqFuCC" target="_blank">114 81 63109</a>
    <small>Copyright©2013 SM ENTERTAINMENT Co., Ltd. ©All rights reserved.</small>
  </address>

  <pre>
  ____  ∧ ∧
   |＼ /(´～`)＼<변화구
   |　|￣￣￣￣￣|
   |　|＝みかん＝|
    ＼|＿＿＿＿＿|
  <pre>

  <p>다음은 패널(Panel) 생성자 함수(Constructor Function) 입니다.</p>

  <pre>
  <code>
    function Panel(element, canClose, closeHandler) {
      this.element = element;
      this.canClose = canClose;
      this.closeHandler = function () { if (closeHandler) closeHandler() };
    }
  </code>
  <pre>
  ```
  
<br>


#### [임베디드 요소]

  - ```<img>``` 요소
    ```
    HTML 문서에 이미지를 포함(링크)

    [속성]
    src    - 이미지 파일 경로 설정
    alt    - 이미지 대체 텍스트 설정
    width  - 이미지 너비 설정
    height - 이미지 높이 설정
    usemap - 이미지 맵 연결 설정
    ```

  - ```<picture>``` 요소 (여러개의 사진) 웃는 고양이 예제
    ```html
    0개 이상의 <source> 요소와 1개 이상의 <img>를 포함하는 컨테이너 요소.
    다양한 스크린 환경에 맞는 적합한 이미지를 제공하기 위한 목적으로 사용.
    <source> 요소를 사용할 수 없을 경우, <img> 요소가 화면에 표시.

    [사용 예시]
    media 속성:
    <picture>
      <source srcset="bamboo-pen.png" media="(min-width: 600px)">
      <img src="bamboo-pen-narrow.png" alt="Bamboo Pen">
    </picture>

    type 속성:
    <picture>
      <source srcset="bamboo-pen.svg" type="image/svg+xml">
      <img src="bamboo-pen-narrow.png" alt="Bamboo Pen">
    </picture>
    ```

  - ```<source>``` 요소
    ```html
    <picture>, <audio>, <video> 요소의 다중 미디어 리소스를 지정하기 위해 사용.

      [사용 예시]
      <video src="videofile.mp4" poster="posterimage.jpg" controls>
        <source src="videofile.webm" type="video/webm">
        <source src="videofile.ogg" type="video/ogg">
        <source src="videofile.mov" type="video/quicktime">
        HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
        <a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
      </video>
    ```

  - ```<video>``` 요소
    ```html
    동영상 콘텐츠를 HTML 문서에 포함하기 위해서 사용.
    src 속성이나 <source> 요소을 이용해 여러 개의 동영상 소스 중 하나를 표시.

    [사용 예시]
    <video src="videofile.mp4" poster="posterimage.jpg">
      HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
      <a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
    </video>

    [속성]
    src      - 비디오 파일 경로
    poster   - 포스터 이미지 경로
    preload  - 사용자 경험 향상(메타데이터 / 비디오 다운로드)에 관한 설정 [none, metadata, auto]
    controls - 재생 컨트롤 표시 설정
    autoplay - 자동 재생 설정
    loop     - 반복 설정
    muted    - 음소거 설정
    ```

  -  ```<audio>``` 요소
      ```html
      동영상 콘텐츠를 포함하기 위해서 사용.
      src속성이나 <source> 요소을 이용해 여러개의 동영상 소스를 표시.

      [사용 예시]
      <audio src="audiofile.mp3">
        HTML5 <code>audio</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
        <a href="http://outdatedbrowser.com/ko">최신형 브라우저로
        업데이트</a>로 업데이트 하세요.
      </audio>

      [속성]
      src      - 오디오 파일 경로
      volume   - 볼륨 조절(0.0 ~ 1.0)
      muted    - 음소거 설정
      poster   - 포스터 이미지 경로
      preload  - 사용자 경험 향상(메타데이터 / 비디오 다운로드)에 관한 설정 [none, metadata, auto]
      controls - 재생 컨트롤 표시 설정
      autoplay - 자동 재생 설정
      loop     - 반복 설정
      ```

  - ```<track>``` 요소
    ```html
    비디오/오디오 재생 시, 자막을 표시.
    default 속성을 설정하지 않을 경우, 자막 사용 안함 됨

    [사용 예시]
    <video src="videofile.mp4" poster="posterimage.jpg">
      <track kind="subtitles" src="videofile.ko.vtt" srclang="ko" label="한국어" default>
      <track kind="subtitles" src="videofile.en.vtt" srclang="en" label="English">
    </video>

    <audio src="audiofile.mp3">
      <track kind="subtitles" src="audiofile.ko.vtt" srclang="ko" label="한국어">
      <track kind="subtitles" src="audiofile.en.vtt" srclang="en" label="English">
    </audio>
    ```

  - ```<iframe>``` 요소
    ```html
    인라인 프레임(Inline Frame)에 다른 HTML 페이지를 포함하여 화면에 표시.

    [사용 예시]
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/0wlXaHmmOVc?rel=0&amp;showinfo=0"
      allow="autoplay; encrypted-media"
      allowfullscreen></iframe>

    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d12643.636820892792!2d127.01610674058901!3d37.6042
      9582641849!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357cbc91e5ca4f03%3A0x18820a16e406c8ea!2z7ISc7
      Jq47Yq567OE7IucIOyEseu2geq1rCDquLjsnYwx64-ZIDUzMC0zNg!5e0!3m2!1sko!2skr!4v1520001155674" width="600"
      height="450"
      style="border: 0"
      allowfullscreen></iframe>

    [속성]
    src             - 프레임 소스 설정
    width           - 프레임 너비 설정
    height          - 프레임 높이 설정
    allowfullscreen - 프레임 전체화면 설정

    ```

  - ```<map>``` 요소
    ```html
    이미지 맵(클릭 가능한 링크 영역)을 정의하기 위해 <area>와 함께 사용됨.

    [사용 예시]
    <img src="products-map.jpg" alt="제품 모음" usemap="#products-map">
    <map name="products-map">
      <area
        shape="circle"
        coords="200,250,25"
        hreflang="en-GB"
        href="another.html"
        alt="Another Page"
        target="_blank">
    </map>
    ```

  - ```<area>``` 요소
    ```html
    이미지의 핫스팟 지역 정의, 하이퍼링크 설정. <map> 내부에서만 사용 가능.

    [속성]
    shape    - 핫스팟 모양 설정
    coords   - 모양의 좌표 값 설정
    href     - 하이퍼링크 주소 설정
    target   - 새 창(탭) 열림 설정
    alt      - 대체 텍스트 설정
    hreflang - 연결된 페이지의 언어 속성 설정
    download - canvas 데이터 다운로드 설정
    ```

  - ```<svg>``` 요소
    ```html
    확장가능한 벡터 그래픽(SVG)은 2차원의 벡터 그래픽을 기술하기 위한 XML 마크업 언어.

    [예시 코드]

    <img src="svgfile.svg" alt="SVG File">

    <svg width="150" height="150" viewBox="0 0 150 150">
      <circle r="50" cx="75" cy="75" fill="#333" stroke="#900" stroke-width="4" />
    </svg>
    ```

    실습 

    ```html 
     <img 
        src="media/image/bang-olufsen.svg"
        alt="Bang Olufsen"
        width="150"
        height="150">

     <svg width="150" height="150">
      <circle cx="75" cy="75" r="40" />
      <circle cx="75" cy="75" r="20" fill="#ff0" />
     </svg>

     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 306 306">
      <style>
        .cls-1 {
          fill: none;
        }

        .cls-2 {
          fill: #aaacae;
        }
      </style>
      <g>
        ~~
      </g>
       </svg>
    ```

</details>

---------------------------------------

<details id="4day">
  <summary>4일차 학습</summary>
  

#### [테이블 요소]

 - ```<table>``` 요소
    ```
    테이블 몸체에 해당되며, 행(row)/열(column) 및 셀(cell)을 포함한다.
    복잡한 내용을 x, y축에 따라 이해하기 쉽게 데이터를 구조화하는데 테이블을 사용한다.
    가장 좋은 테이블 디자인은 최대한 단순하게 표를 구성하는 것이다.
    테이블 내 테이블을 중첩해서는 안된다.
    테이블을 레이아웃(배치) 목적으로 사용해서는 안된다.
    border 속성을 사용해 테두리를 그릴 수 있다. (CSS로 대체하는 것이 좋다)
    ```

 - ```<caption>``` 요소
    ```
    테이블의 제목을 명시적으로 제공하며, 제작자는 표의 내용을 이해할 수 있도록 정보를 제공해야 함.
    테이블 내용이 복잡해 설명이 필요하다면 아래 나열된 방법 중 하나를 선택해 기술해야 한다.

      [설명(summary)을 추가하는 방법]
        1. aria-describedby 속성을 사용해 설명 단락(paragraph)을 연결
        2. <figure> 요소에 aria-labelledby 속성을 사용해 제목(caption)을 연결
    ```

 - ```<tr>``` 요소
  
    ```
      테이블의 행(row)을 말하며 내부에 셀 제목(header), 셀 내용(data)을 포함한다.
    ```

 - ```<th>``` 요소

    ```
    테이블 셀 제목(header cell in a table)으로 행(tr) 내부에 포함되어야 한다.

    [속성]
      scope: 행(row) 또는 열(col), 행그룹(rowgroup), 열그룹(colgroup)의 제목임을 명시
      abbr: 제목이 길어 축약(Abbreviation)이 필요할 때 사용
      colspan: 열(column)을 그룹 지을 때 사용
      rowspan: 행(row)을 그룹 지을 때 사용
    ```

 - ```<td>``` 요소
    ```
    테이블 셀 내용(data cell in a table)으로 행(tr) 내부에 포함되어야 한다.

    [속성]
      colspan: 열(column)을 그룹 지을 때 사용
      rowspan: 행(row)을 그룹 지을 때 사용
      headers: 셀 제목을 하나 이상 연결하여 읽기 용이하도록 구성할 때 사용
    ```

 - ```<thead>``` 요소
    ```
    테이블 행 블록(row block) 내에 제목 열 그룹(column headers)으로 구성할 경우 사용한다.
      선택적(option)으로 사용한다. (필수 아님)
    ```

 - ```<tbody>``` 요소
    ```
    행 블록 내에 테이블 데이터로 구성할 때 사용한다.
    선택적(option)으로 사용한다. (필수 아님)
    ```

 - ```<tfoot>``` 요소
    ```
    행 블록 내에 열 요약(column summaries)로 구성할 때 사용한다.
    선택적(option)으로 사용한다. (필수 아님)
    ```

 - ```<col>``` 요소
    ```
    테이블 열(column)을 하나 이상 묶고자 할 때 사용한다.
    일반적으로 colgroup 요소 내부에 포함시킨다.
    선택적(option)으로 사용한다. (필수 아님)

    [속성]
      span: 열 묶음 개수 설정
    ```
 - ```<colgroup>``` 요소
    ```
    테이블 열(column) 그룹을 만들고자 할 때 사용한다.
    내부에 col 요소를 포함하거나, 포함하지 않을 수 있다.
    선택적(option)으로 사용한다. (필수 아님)

    [속성]
      span: colgroup 요소가 col을 포함하지 않을 경우, 열 묶음 개수 설정
    ```

  실습 

  - table내에 tody를 안 적어줘도 자동으로 생깁니다.
  - 열은 꼭 맞쳐야합니다.
  - th에는 스크린 리더로 알 수 있게 scope="row" 라는 것을 넣어주어야 합니다. 
  - aria-describedby="" 자세한 내용을 기술하기 위해 사용. 표에 대한 자세한 내용 전달
  - table border 속성은 css를 사용하여 표현해 주는 것이 좋다.

    ```
    <p id="compare-shoes-table"> 국제(한국, 미국, 영국, 유럽) 성인 남성 운동화 사이즈 비교 표로 4행 
    12열로 구성되어 있습니다.
    <table border="1" aria-describedby="compare-shoes-table">
    ```


    ```html
    <table border="1">
      <cation>성인 남성 운동화 사이즈표</cation>
      <tr>
        <th>한국(mm)</th> 
        <td>240</td> 
        <td>245</td>
        <td>250</td>
        <td>255</td>
        <td>260</td>
        <td>265</td>
        <td>270</td>
        <td>275</td>
        <td>280</td>
        <td>285</td>
        <td>290</td>
      </tr>
      <tr>
        <th>미국(US)</th> 
        <td>6</td>
        <td>6.5</td>
        <td>7</td>
        <td>7.5</td>
        <td>8</td>
        <td>8.5</td>
        <td>9</td>
        <td>9.5~10</td> 
        <td>10~10.5</td>
        <td>11</td>
        <td>11.5</td>
      </tr>
      <tr>
        <th>영국(UK)</th> 
        <td>5</td>
        <td>5.5</td> 
        <td>6</td> 
        <td>6.5</td> 
        <td>7</td> 
        <td>7.5</td> 
        <td>8</td> 
        <td>8.5~9</td> 
        <td>9~9.5</td> 
        <td>10</td> 
        <td>11</td>
      </tr>
      <tr>
        <th>유럽(EU)</th> 38~39 39 40 40~41 41 42 42~43 43 44 44~45 45
      </tr>
    </table>
    ```

  - ```<thead>``` 행 블록을 만들때 사용
  - scope 속성 'rowgroup' 가로그룹 'colgroup' 세로 그룹 (행인지 열인지 아니면 행의 그룹인지 열의 그룹인지 설정해줍니다.)
  - ```<th>```  해당 그룹의 제목
  - td header 속성 **

    ```html
      <table id="real-deal-table" border="1" aria-describedby="real-deal-table-summary">
      <caption>
        <strong>
          최근 3개월간 실거래가
          <button type="button" class="open-tooltip" title="자세히" aria-label="자세히">?</button>
        </strong>
          <!-- ? -->
        <div id="real-deal-table-summary" class="a11y-hidden">
          <h3>국토교통부 실거래가</h3>
          <p>
            제공: 국토교통부<br>
            최근 3개월간(2018.01월~03월) 신고된 국토교통부 실거래 가격자료를
            기반으로 최저가격과 최고가격 및 거래건수를 노출합니다.
          </p>
          <button type="button" class="close-tooltip" title="닫기" aria-label="닫기">X</button>
        </div>
        
        <!-- URL 주소: https://goo.gl/FxWHEg -->
        <p>실거래가 기준: 2018.03 <a href="https://goo.gl/FxWHEg" target="_blank">자료: 국토교통부</a></p>
      </caption>
      
      <thead>
        <tr>
          <th id="rd-1" rowspan="2" scope="col">공급/전용(㎡)</th>
          <th id="rd-2" colspan="3" scope="colgroup">매매 실거래가(만원)</th>
          <th id="rd-3" colspan="3" scope="colgroup">전세 실거래가(만원)</th>
          <th id="rd-4" colspan="3" scope="colgroup">월세 실거래가(만원)</th>
        </tr>
        <tr>
          <th id="rd-2-1" scope="col">최저가</th>
          <th id="rd-2-2" scope="col">최고가</th>
          <th id="rd-2-3" scope="col">거래건수</th>
          <th id="rd-3-1" scope="col">최저가</th>
          <th id="rd-3-2" scope="col">최고가</th>
          <th id="rd-3-3" scope="col">거래건수</th>
          <th id="rd-4-1" scope="col">최저가</th>
          <th id="rd-4-2" scope="col">최고가</th>
          <th id="rd-4-3" scope="col">거래건수</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th id="rd-1-1" scope="row">80/59.91</th>
          <td headers="rd-1 rd-1-1 rd-2" colspan="3">-</td>
          <td headers="rd-1 rd-1-1 rd-3 rd-3-1">43,000(2층)</td>
          <td headers="rd-1 rd-1-1 rd-3 rd-3-2">43,000(2층)</td>
          <td headers="rd-1 rd-1-1 rd-3 rd-3-3">1</td>
          <td headers="rd-1 rd-1-1 rd-4" colspan="3">-</td>
        </tr>
        <tr>
          <th id="rd-1-2" scope="row">84/59.99</th>
          <td headers="rd-1 rd-1-2 rd-2 rd-2-1">47,800(4층)</td>
          <td headers="rd-1 rd-1-2 rd-2 rd-2-2">55,000(22층)</td>
          <td headers="rd-1 rd-1-2 rd-2 rd-2-3">10</td>
          <td headers="rd-1 rd-1-2 rd-3 rd-3-1">43,000(2층)</td>
          <td headers="rd-1 rd-1-2 rd-3 rd-3-2">43,000(2층)</td>
          <td headers="rd-1 rd-1-2 rd-3 rd-3-3">1</td>
          <td headers="rd-1 rd-1-2 rd-4 rd-4-1">5,000/120(6층)</td>
          <td headers="rd-1 rd-1-2 rd-4 rd-4-2">40,000/10(4층)</td>
          <td headers="rd-1 rd-1-2 rd-4 rd-4-3">5</td>
        </tr>
        <tr>
          <th id="rd-1-3" scope="row">111/84.82</th>
          <td headers="rd-1 rd-1-3 rd-2 rd-2-1">63,200(12층)</td>
          <td headers="rd-1 rd-1-3 rd-2 rd-2-2">63,500(19층)</td>
          <td headers="rd-1 rd-1-3 rd-2 rd-2-3">2</td>
          <td headers="rd-1 rd-1-3 rd-3 rd-3-1">53,000(13층)</td>
          <td headers="rd-1 rd-1-3 rd-3 rd-3-2">53,000(13층)</td>
          <td headers="rd-1 rd-1-3 rd-3 rd-3-3">1</td>
          <td headers="rd-1 rd-1-3 rd-4" colspan="3">-</td>
        </tr>
        <tr>
          <th id="rd-1-4" scope="row">112/84.92</th>
          <td headers="rd-1 rd-1-4 rd-2 rd-2-1">65,000(6층)</td>
          <td headers="rd-1 rd-1-4 rd-2 rd-2-2">65,000(6층)</td>
          <td headers="rd-1 rd-1-4 rd-2 rd-2-3">1</td>
          <td headers="rd-1 rd-1-4 rd-3 rd-3-1">52,000(10층)</td>
          <td headers="rd-1 rd-1-4 rd-3 rd-3-2">52,000(10층)</td>
          <td headers="rd-1 rd-1-4 rd-3 rd-3-3">1</td>
          <td headers="rd-1 rd-1-4 rd-4" colspan="3">-</td>
        </tr>
        <tr>
          <th id="rd-1-5" scope="row">112/84.94</th>
          <td headers="rd-1 rd-1-5 rd-2 rd-2-1">60,000(25층)</td>
          <td headers="rd-1 rd-1-5 rd-2 rd-2-2">60,000(25층)</td>
          <td headers="rd-1 rd-1-5 rd-2 rd-2-3">1</td>
          <td headers="rd-1 rd-1-5 rd-3 rd-3-1">45,000(10층)</td>
          <td headers="rd-1 rd-1-5 rd-3 rd-3-2">45,000(10층)</td>
          <td headers="rd-1 rd-1-5 rd-3 rd-3-3">1</td>
          <td headers="rd-1 rd-1-5 rd-4 rd-4-1">35,000/60(5층)</td>
          <td headers="rd-1 rd-1-5 rd-4 rd-4-2">35,000/60(5층)</td>
          <td headers="rd-1 rd-1-5 rd-4 rd-4-3">1</td>
        </tr>
        <tr>
          <th id="rd-1-6" scope="row">145/114.98</th>
          <td headers="rd-1 rd-1-6 rd-2 rd-2-1">76,800(15층)</td>
          <td headers="rd-1 rd-1-6 rd-2 rd-2-2">80,000(14층)</td>
          <td headers="rd-1 rd-1-6 rd-2 rd-2-3">2</td>
          <td headers="rd-1 rd-1-6 rd-3 rd-3" colspan="3">-</td>
          <td headers="rd-1 rd-1-6 rd-4 rd-4-1">5,000/200(5층)</td>
          <td headers="rd-1 rd-1-6 rd-4 rd-4-2">5,000/200(5층)</td>
          <td headers="rd-1 rd-1-6 rd-4 rd-4-3">1</td>
        </tr>
      </tbody>
    </table>
    ```

  
<br>


#### [폼 요소]
  - ```<form>``` 는 처음에는 method의 기본 값이 get 입니다. (개발자와 협의를 해서 어떤 주소로 넣어 줄까 물어봐야합니다.)
  - post인 경우 민감한 정보 데이터, 이메일, 개인정보 같은 것을 전송할 때 사용.

      ```html
      <form action-"/" method="POST" enctype="multpart-formdata">
        <p>
          <label for="user_name">이름</label>
          <input id="user_name"
            name="user_name" 
            type="text" 
            placeholder="주" 
            maxlength="4" 
            readonly 
            value="정소하" 
            minlength="2"
          </p>
          <p>
            <label for="user_pass">비밀번호</label>
            <input
              type="password"
              name="user_pass"
              id="user_pass"
              required
              placeholder="비밀번호 6자리 입력해주세요."
          </p>
          <p>
            <label><input type="radio" name="user_gender" value="1">남성</label>
            <label><input type="radio" name="user_gender" value="2" checked>여성</label>
          </p>
          <p>
            <label><input type="checkbox" name="user_agree" id="user_agree">모든 내용을 읽고 동의합니까?</label>
          </p>
          <p>
            <input type="file" name="user_data_upload" id="user_data_upload">
          </p>
          <p>
            <label>검색<input type="search" name="user_search" id="user_search"></label>
          </p>
          <p>
            <label>이동할 웹주소<input list="url_ex" type="url" name="user_url" id="user_url"></label>
            <datalist id="url_ex">
              <option value="http://naver.com">naver.com</option>
              <option value="http://nate.com">nate</option>
              <option value="http://google.com">google</option>
              <option value="http://goo.gl">google. short url</option>
            </datalist>
          </p>
          <p>
            <label>전화번호<input list="tel_ex" type="tel" name="user_tel" id="user_tel"></label>
             <datalist id="tel_ex">
              <option value="111">111</option>
              <option value="222">222</option>
              <option value="333">333</option>
              <option value="444">444</option>
            </datalist>
          </p>
          <p>
            <label>이메일<input type="email" name="user_email" id="user_email"></label>
          </p>
          <p>
            <label for="user_hobby">취미</label>
            <select name="user_hobby" id="user_hobby">
              <option value="0">없음</option>
              <option value="1">축구</option>
              <option value="2">독서</option>
              <option value="3">영화관람</option>
            </select>
          </p>
          <input type="submit" value="전송">
          <input type="button" value="버튼">
          <input type="image" src="https://goo.gl/Ng66oQ" alt="체크인" width="20" height="20">
          <input type="reset" value="초기화">
          <input type="hidden" name="using-ajax" value="true">
          <input type="number" name="" id="" min="100" step="10" max="1000" value="150">
          <input type="range" name="" id="" min="10" step="5" max="25" value="15">
          <input type="color" name="" id="" value="#F7CC60">
          <button type="reset">초기화</button>
          <button type="submit">전송</button>
      </form>

      사용자의 데이터를 입력 받을 수 있는 폼 컨트롤을 말함.
      다양한 유형(Type) 설정이 가능하며, 유형에 맞는 역할을 수행한다.

      [사용 예시]
      <form action="https://formspree.io/your@email.com" method="POST">
        ...
      </form>
      ```

  - ```input``` 사용자의 데이터를 입력받을 수 있는 폼 컨트롤러입니다. 기본값은 text입니다.
  - input만 있으면 어떤 것인지 모르기 때문에 label 요소를 사용해 줘야 합니다.
  - placeholder 기능을 이용해서 텍스트에 어떤 것을 사용해야 할지 알려줍니다.
  - required 필수 요소를 설정할 수 있습니다.
  - optgroup으로 셀렉트 들을 묶어 줄 수 있습니다.. disabled 라는 속성을  사용하게 되면 선택이 안되게 설정이 가능합니다.
  - fieldset으로 묶고 제목을 legend로 묶게되면 해당 폼들은 묶이게 됩니다.
  - progres태그 smeter태그

    ```
    <input>
    사용자의 데이터를 입력 받을 수 있는 폼 컨트롤을 말함.
    다양한 유형(Type) 설정이 가능하며, 유형에 맞는 역할을 수행한다.

    [속성]
      - name
      - placeholder
      - value-
      - readonly
      - required
      - disabled
      - minlength
      - maxlength
      - list

    [유형]
      - text
      - password
      - checkbox
      - radio
      - file
      - submit
      - button
      - image
      - reset
      - hidden
      - search
      - url
      - tel
      - email
      - date
      - month
      - week
      - time
      - datetime-local
      - number
      - range
      - color

    <label>
    - 컨트롤에 레이블(이름)을 붙이고자 할 경우 사용.

    [사용 예시]

      1. <label>이름 <input type="text" placeholder="이두연"></label>

      2. <label for="u_pass">비밀번호</label>
         <input id="u_pass" name="u_pass" type="password" maxlength="8" placeholder="비밀번호 8자리를 입력해주세요">

  <button>
    - 버튼 폼 컨트롤로 사용자의 인터랙션을 받아 액션을 트리깅(방아쇠) 처리함.

    [type]
      - submit (초기 값)
      - button
      - reset

      [사용 예시]
        <button type="submit">전송</button>
        <button type="button">버튼</button>
        <button type="reset">초기화</button>

  <select>
    - 드롭 다운 메뉴(옵션을 선택 할 수 있는) 컨트롤을 말함.
      내부에 <option> 요소를 포함하여 사용자에게 선택할 수 있도록 한다.
      <option>을 묶어 그룹으로 만들고자 한다면 <optgroup> 요소를 사용하고,
      label 속성을 사용해 그룹 이름을 설정한다.

      [속성]
        - name
        - multiple
        - disabled
        - required
        - size

      [사용 예시]
        <label for="user_hobby">취미</label>
        <select name="user_hobby" id="user_hobby">
          ...
        </select>

  <option>
    - <select>, <datalist>, <optgroup> 내부에 포함 가능한 컨트롤로 항목을 만드는데 사용됨.

    [속성]
      - value
      - selected
      - label
      - disabled

    [사용 예시]
      <label for="user_hobby">취미</label>
      <select name="user_hobby" id="user_hobby" required>
        <option value="0">없음</option>
        <option value="1" selected>축구</option>
        <option value="2" label="basketball" disabled>농구</option>
        <option value="3">독서</option>
        <option value="3">영화관람</option>
      </select>

  <optgroup>
    - <option> 컨트를을 그룹지을 때 사용됨.

    [속성]
      - disabled
      - label

    [사용 예시]
      <p>
        <label for="user_hobby">취미</label>
        <select name="user_hobby" id="user_hobby" required>
          <option value="0">없음</option>
          <optgroup label="구기종목">
            <option value="1" selected>축구</option>
            <option value="2" label="basketball" disabled>농구</option>
          </optgroup>
          <optgroup label="문화생활" disabled>
            <option value="3">독서</option>
            <option value="3">영화관람</option>
          </optgroup>
        </select>
      </p>

  <textarea>
    - 멀티라인 일반 텍스트 편집 컨트롤을 말한다.

    [속성]
      - name
      - placeholder
      - rows
      - cols
      - readonly
      - required
      - disabled
      - minlength
      - maxlength

    [사용 예시]
      <div>
        <label for="user_comments">코멘트</label>
        <p>
          <textarea name="user_comments" id="user_comments" cols="24" rows="5">남기고 싶은 말을 
          작성해주세요.</textarea>
        </p>
      </div>

  <fieldset>
    - 하나 이상의 폼 컨트롤을 그룹화 하는데 사용됨.

    [속성]
      - name
      - disabled

    [사용 예시]
      <fieldset name="user_acount">
        ...
      </fieldset>

  <legend>
    - <fieldset> 컨트롤의 레이블(이름)을 설정하는 컨트롤.

    [사용 예시]
      <fieldset name="user_acount">
        <legend>사용자 계정</legend>
      </fieldset>

  <output>
    - 계산된 결과를 출력하는 컨트롤.

    [속성]
      - name
      - for

    [사용 예시]
      <form oninput="result_sum.value = parseInt(n1.value + n2.value, 10)">
        <p>
          <input type="number" name="n1" value="4"> +
          <input type="number" name="n2" value="10"> =
          <output name="result_sum">14</output>
        </p>
      </form>

  <datalist>
    - 데이터 목록 요소 컨테이너 컨트롤.
      내부에 <option> 요소를 사용해 항목을 만든다.

      [사용 예시]
        <label>이동할 웹주소 <input list="url_ex" type="url" name="user_url" id="user_url"></label>
        <datalist id="url_ex">
          <option value="http://naver.com">naver</option>
          <option value="http://nate.com">nate</option>
          <option value="http://google.com">google</option>
          <option value="http://goo.gl">google short url</option>
        </datalist>

  <progress>
    - 작업의 완료 진행 상황을 표시하는데 사용되는 컨트롤.

    [속성]
      - value
      - max

    [사용 예시]
      <progress value="10" max="100">10%</progress>

  <meter>
    - 알려진 범위 내에서의 스칼라 측정 또는 분포 비율을 나타내는 컨트롤. (게이지(gauge)라고도 불림)
      디스크 사용 현황, 쿼리 결과의 관련성, 특정 후보에 대한 투표율 등이 해당됨.

    [속성]
      - value
      - min
      - max
      - low
      - high
      - optimum

    [사용 예시]
      <meter value="20" min="5" max="40">20</meter>
    ```
</details>

---------------------------------------

<details id="5day">
  <summary>5일차 학습</summary>

#### [인터랙티브 요소]
  - ```<deatils>``` 예전 강의에서 sup를 이용해서 각주로 만든적이 있다. 하지만 details는 각주의 용도로 적합하지 않다.
  - open 속성을 넣어주면 details 요소가 펼쳐서 보여줍니다.
  - 원하는 제목을 표시하고 싶으면 summery를 사용할 수 있습니다.

  ```html
  <details open>
    <summary>서용자
    <p>
      디스클로저 위젯(disclosure widget, 참고: https://goo.gl/uznvFY)으로 정보를 감추거나, 펼쳐서 보여준다.
      모든 정보를 일시에 공개하지 않고 사용자의 요구에 맞춰 정보를 공개할 수 있다. (화면의 복잡함을 줄임)
      아코디언(Accordion) 컴포넌트와 비슷하게 작동한다.
    </p>
  </details>
  ```

  ```html
  <div class="container">
    <dialog>
      <button type="submit">confirm</button>
    </dialog>
  </div>
  ```

  ```html
  <style>
    body {
      margin: 0;
      min-height: 100vh;
    }
    .demo {
      display: flex;
      justify-content: center;
      align-items: flex-start;
    }
    .container {
      margin-top: 200px;
      width: 80%;
    }

    .dialog {
      max-width: 415px;
      width: 80%;
      border: 2px solid #3b99fc;
      border-radius: 6px;
      box-shadow: 1px 7px 11px rgba(118, 118, 118, 0.32);
    }
    .dialog-headline {
      margin: 0 0 20px;
      font-size: 24px;
      font-weight: 400;
    }
    .dialog summary {
      width: 100%;
    }
    .dialog dl {
      margin-top: 20px;
      margin-bottom: 0;
      border-top: 1px solid #3b99fc;
      padding-top: 20px;
    }
    .dialog dt {
      float: left;
      width: 145px;
      margin-right: 10px;
    }
    .dialog dd {
      margin-left: 0;
      margin-bottom: 5px;
    }
  </style>

  <div class="container">
    <dialog class="dialog" open>
      <section>
        <h2 class="dialog-headline">"html5.2-video-recture.mp4" 파일복사</h2>
        <details>
          <summary> 복사중... <progress value="25" max="100"></progress> 25% </summary>
          <dl>
            <dt>초당 전송 속도:</dt><dd>723KB</dd>
            <dt>로컬 파일이름: </dt><dd>/Desktop/html5.2-vidio-recture.mp4</dd>
            <dt>원격 파일이름: </dt><dd>?Backup/html5.2-video-recture.mp4</dd>
            <dt>재생시간: </dt><dd>00:14:38</dd>
            <dt>컬러 프로파일</dt><dd>HD (1-1-1)</dd>
            <dt>해상도(너비x높이)</dt><dd>1680x1050</dd>
          </dl>
        </details>
    </dialog>
  </div>

  ```


  ```html
 <details> 요소
  - 디스클로저 위젯(disclosure widget, 참고: https://goo.gl/uznvFY)으로 정보를 감추거나, 펼쳐서 보여준다.
    모든 정보를 일시에 공개하지 않고 사용자의 요구에 맞춰 정보를 공개할 수 있다. (화면의 복잡함을 줄임)
    아코디언(Accordion) 컴포넌트와 비슷하게 작동한다.

    참고로 각주(footnote)에는 적합하지 않다.

  [속성]
    open - 페이지 로딩 시, 위젯을 펼쳐 표시하도록 설정

  [사용 예시]
    <details open>
      ...
    </details>

  <summary> 요소
  - <details> 요소의 레이블/캡션(제목), 서머리(요약) 등을 표시한다.
    폼 <fieldset> 요소의 제목을 <legend>가 표시하듯 비슷하다.

  [사용 예시]
    
    <section class="progress window">
      <h1>"Really Achieving Your Childhood Dreams" 파일 복사</h1>
      <details>
      <summary>복사중... <progress max="375505392" value="97543282"></progress> 25%</summary>
      <dl>
        <dt>초당 전송 속도:</dt>
        <dd>452KB/s</dd>
        <dt>로컬 파일이름:</dt>
        <dd>/home/rpausch/raycd.m4v</dd>
        <dt>원격 파일이름:</dt>
        <dd>/var/www/lectures/raycd.m4v</dd>
        <dt>재생시간:</dt>
        <dd>01:16:27</dd>
        <dt>컬러 프로파일:</dt>
        <dd>SD (6-1-6)</dd>
        <dt>영상 크기(너비×높이):</dt>
        <dd>640×480</dd>
      </dl>
      </details>
    </section>
  ```

<br>


#### [스크립팅 요소들]

  - HTML에서는 자바스크립트라고 입력을 안해도 자바 스크립트라고 인식하기 때문에 따로 명시할 필요가 없습니다. type="application/ecmascript
  - LINK 태그에 rel 관계성 stylesheet를 명시
  - 크롬 설정에서 debugger에서 disable javascript를 사용하게 되면 자바스크립트가 안되게 환경을 잡아줄 수 있습니다.
  - canvas는 API가 방대하고 비트맵을 그릴 때 사용합니다.

  ```javascript
  js/app.js

  console.log('<script> 요소를 사용해 js/app.js 파일을 HTML 문서에 읽어들였습니다.');
  var bgColor = window.prompt('문서의 배경 색상을 입력해주시겠습니까?', '#eced00');
  document.querySelector('body').style.cssText = 'background: ' + bgColor;
  console.log('<body> 요소에 CSS 스타일을 적용하여 배경 색을 ' + bgColor + ' 색상으로 변경 처리했습니다.');
  ```

  ```css
  css/app.css

  html {
    background: #222;
    height: 100%;
  }

  body {
    height: 50%;
    margin: 0;
  } 
  ```

  ```html
  <link rel="stylesheet" href="css/app.css">

  ```

  ```html
  <stlye>
    body {
       background-color:#96e72a; 
       margin:0; 
       min-height: 100vh; 
       width: 100ww
    }
  </stlye>

  <body>

  <scrpt src="js/app.js"></script>

  <script>
    // JavaScript 코드
    console.log('JavaScript 코드를 실행했습니다.');
    console.log(document.characterSet);
    console.log(document.doctype);
  </script>

  <noscript>
    <p>JavaScript를 지원하지 않습니다.</p>
  <noscript>
  ```

  ```html
 <noscript> 요소
    - 사용자의 웹 브라우저 환경에서 스크립트를 지원되지 않거나, 스크립트가 꺼져있는 경우, 문서에 표시될 문구를 삽입한다.

    [코드 예시]
      <noscript>
        <p>JavaScript를 지원하지 않습니다.</p>
      </noscript>


  <canvas> 요소
    - JavaScript를 사용하여 그래픽(비트맵)을 그릴 때 사용한다.
      <canvas> 요소로부터 2D 또는 WebGL 컨텍스트 객체를 추출해 그래픽을 그릴 수 있다.

    [코드 예시]

      <canvas width="800" height="600"></canvas>

      <script>
        // canvas 드로잉
        var canvas = document.querySelector('canvas');
        var ctx = canvas.getContext('2d');
        ctx.translate(200, 40);
        ctx.beginPath();
        ctx.moveTo(180, 175);
        ctx.fillStyle = '#ff0';
        ctx.arc(180, 175, 60, Math.PI * -0.35, Math.PI * -1.05, true);
        ctx.fill();
        ctx.beginPath();
        ctx.moveTo(190, 190);
        ctx.fillStyle = '#ff0';
        ctx.arc(190, 190, 100, Math.PI * -0.35, Math.PI * 0.95);
        ctx.fill();
      </script>

  ```

<br>

#### [유저 인터랙션 속성]
  
  - tabIndex="0"는 포커스를 가질수 없는 요소 이지만 포커스를 가질수 있게해준다. -1을 속성값으로 할시 포커스에서 제외할 수 있습니다.
  - 이미지는 포커스 요소가 아니지만 탭으로 포커스가 가능하게 할 수 있습니다
  - 해당 tabIndex 속성을 해당 요소에 포커스를 없앴다가 생기게 자바스크립트로 해서 유용한 개발을 할 수 있습니다.
  - 논리적 흐름을 방해하지 않도록 해야한다. 위에 나온 흐름대로 해야 한다. tabIndex는 양수를 안 사용 하는 것이 좋다.

  - accessKey같은 경우 사용자 경험이 다릅니다.
  - accessKey는 키보드 단축키를 사용할 수 있다.

  ```
  hidden 속성
      - 모든 HTML 요소들은 hidden 속성을 가질 수 있으며, 요소에 설정되면 요소가
        아직 페이지의 현재 상태와 직접적으로 관련이 없거나 페이지의 다른 부분에서
        내용을 재사용하도록 선언하는 데 사용된다. 브라우저는 hidden 속성이 설정된
        요소를 화면에 렌더링하지 않는다.

        [사용 예시]
          <h1>hidden 속성 사용 예</h1>
          <section id="login">
            <h2>로그인</h2>
            <form>
            ...
            </form>
            <script>
              function login() {
                // 화면 변경
                document.querySelector('#login').hidden = true;
                document.querySelector('#game').hidden  = false;
              }
            </script>
          </section>
          <section id="game" hidden>
            <h2>게임 시작</h2>
            ...
          </section>


    tabindex 속성
      - 요소를 키보드로 탐색할 수 있도록 설정하거나, 제외 또는 순서대로 탐색할 수 있도록 설정할 수 있다.
        "탭(Tab) 이동"이란 용어는 순차적 포커스 탐색을 사용하여 포커스 가능(Focusable) 요소 사이를
        이동하는 것을 의미한다.

        [기본적으로 포커스 가능한 요소들](참고: https://allyjs.io/data-tables/focusable.html)
          폼 컨트롤 요소들           : input, button, textarea, select 등
          href 속성을 가진 요소들     : a, area
          controls 속성을 가진 요소들 : video, audio

        [사용 예시]

          // [양수] 탭 포커스 순서(2번째)를 설정한다.
          // (논리적 포커스 흐름에 방해가 되기에 사용을 권장하지 않음)
          <button
            type="button"
            class="button is-play"
            tabindex="2">재생</button>

          // [0] div 요소는 포커스를 가지지 않는 요소이지만, 포커스를 적용할 수 있게 된다.
          // 컴포넌트 제작 시, 비 포커스 요소에 포커스를 적용해야 할 경우 유용하게 사용됨.
          <div tabindex="0"></div>

          // [-1] 일반적인 포커스 순서에서 제외시킬 수 있다.
          // (JavaScript 프로그래밍으로 포커스 처리 가능)
          // 컴포넌트의 일부 요소를 일시적으로 포커스 순서에서 제외한 후,
          // 목표에 따라 포커스를 다시 활성화 처리할 수 있다.
          <ol class="TOC">
            <li><a href="#pinch">위기</a></li>
            <li><a href="#overcome" tabindex="-1">극복</a></li>
          </ol>


    accesskey 속성
      - 모든 HTML 요소는 accesskey 속성을 가질 수있다. 속성 값은 키보드 단축키로 설정된다.
        하지만 accesskey 속성의 단축키는 브라우저와 운영체제 플랫폼에 의존하고 있어 운영체제마다
        사용자 경험이 달라진다. 쉽게 말해 Windows 사용자와 Mac OSX 사용자가 사용하는
        단축키는 달라진다. (iPhone과 Android 사용자 경험이 다른 것처럼)

        [브라우저 × 운영체제 플랫폼]
          Windows
            Chrome  : Alt + 단축키
            IE      : Alt + 단축키
            Safari  : Alt + 단축키
            Opera   : Alt + 단축키
            Firefox : Alt + Shift + 단축키
          Mac OSX
            Chrome  : Control + Alt + 단축키
            Safari  : Control + Alt + 단축키
            Opera   : Control + Alt + 단축키
            Firefox : Control + 단축키
          Linux
            Chrome  : Alt + 단축키
            Opera   : Alt + 단축키
            Firefox : Alt + Shift + 단축키

        [사용 예시]
          <button
            type="button"
            class="button is-collect"
            accesskey="C"
            onclick="collect()">
            수집
          </button>


    contenteditable 속성
      - contenteditable 속성이 설정된 요소는 사용자가 직접 편집할 수 있도록 만들어 준다.
        값이 true 또는 빈 문자열("")일 경우 편집 허용.
        값이 false 일 경우 편집을 허용하지 않음.

        [사용 예시]
        <p contenteditable>
          ...
        </p>


    draggable 속성
      - 모든 HTML 요소는 draggable 속성을 가질 수 있다.
        값이 true 일 경우 드래그(Drag) 가능.
        값이 false 또는 빈 문자열("")일 경우 드래그 불가능.

        [사용 예시]
        <p draggable="true">
          ...
        </p>
  ```

  ```html
  <button type="button" accesskey="V" class="button is-show">컨테이너 표시</button>

  <div class="container">

    <img
      class="drag-element"
      src="images/fashion-model-pose.png"
      alt="패션 모델"
      width="276" height="417">

    <div class="dropzone">
      <p>Drop Zone</p>
    </div>

  </div>
  ```

  ```css
  css/App.css
  <style>
    html, body {
      height: 100%;
    }
    body {
      margin: 0;
    }
    .demo {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .button.is-show {
      cursor: pointer;
      position: fixed;
      top: 40px;
      left: 40px;
      border: 1px solid transparent;
      border-radius: 4px;
      padding: 1em 1.4em;
      font-family: "Spoqa Han Sans";
      font-weight: 400;
      font-size: 15px;
      color: #454545;
      background: #eeeeee;
      transition: all 0.1s ease-out;
    }
    .button.is-show:hover {
      background: #11a981;
      color: #fff;
    }
    .button.is-show:active {
      transform: scale(0.98);
      opacity: 0.8;
    }
    .button.is-show:focus {
      outline: none;
      border-color: #11a981;
    }

    .container {
      display: flex;
      justify-content: space-around;
      align-items: center;
      flex-flow: row wrap;
      width: 100vw;
    }
    .container[hidden] {
      display: none;
    }
    .dropzone {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      width: 400px;
      height: 500px;
      border: 10px solid #eee;
      transition: all 0.24s ease-in-out;
    }
    .dropzone p::selection {
      background: #eee;
      color: #454545;
    }
    .dropzone p {
      position: absolute;
      z-index: -1;
      margin: 0;
      font-size: 56px;
      font-weight: 900;
      color: #eee;
    }
    .drag-element {
      user-select: none;
    }
  </style>
  ```

  ```javascript
  function hiddenDemo() {
    var showButton = document.querySelector('.button.is-show');
    var container  = document.querySelector('.container');
    showButton.addEventListener('click', function(){
      container.removeAttribute('hidden');
    });
  }

  function dragDemo() {

    var draggableEl = document.querySelector('img[draggable="true"]');
    var dropZone    = document.querySelector('.dropzone');

    if (!draggableEl) { return; }

    function onDragStart(e) {
      console.log('드래그 스타트(Drag Start)');
      var src    = e.target.getAttribute('src');
      var alt    = e.target.getAttribute('alt');
      var width  = e.target.getAttribute('width');
      var height = e.target.getAttribute('height');
      e.dataTransfer.setData('src', src);
      e.dataTransfer.setData('alt', alt);
      e.dataTransfer.setData('width', width);
      e.dataTransfer.setData('height', height);
    }

    function onDragOver(e) {
      console.log('드래그 오버(Drag Over)');
      e.preventDefault();
    }

    function onDragEnter(e) {
      console.log('드래그 엔터(Drag Enter)');
      e.preventDefault();
      e.target.style.borderColor = '#11a981';
    }

    function onDragLeave(e) {
      console.log('드래그 리브(Drag Leave)');
      e.preventDefault();
      dropZone.style.borderColor = '#eee';
    }

    function onDragEnd(e) {
      console.log('드래그 엔드(Drag End)');
      e.preventDefault();
      dropZone.style.borderColor = '#eee';
    }

    function onDrop(e) {
      console.log('드롭(Drag Drop)');
      e.preventDefault();
      var src    = e.dataTransfer.getData('src');
      var alt    = e.dataTransfer.getData('alt');
      var width  = e.dataTransfer.getData('width');
      var height = e.dataTransfer.getData('height');
      var img = new Image();
      img.setAttribute('src', src);
      img.setAttribute('alt', alt);
      img.setAttribute('width', width);
      img.setAttribute('height', height);
      e.target.appendChild(img);
      draggableEl.style.opacity = 0;
    }

    var img = null;

    function onKeyUp(e) {
      if ( !img && e.key.toLowerCase() === 'arrowright' ) {
        console.log('오른쪽 방향 화살표(→) 키를 눌렀습니다.');
        img = new Image();
        var target = e.target;
        img.setAttribute('src', target.src);
        img.setAttribute('alt', target.alt);
        img.setAttribute('width', target.width);
        img.setAttribute('height', target.height);
        dropZone.appendChild(img);
        draggableEl.style.opacity = 0;
        draggableEl.setAttribute('tabindex', -1);
        img.addEventListener('keyup', onKeyUp);
        img.setAttribute('tabindex', 0);
      }
      if ( img && e.key.toLowerCase() === 'arrowleft' ) {
        console.log('왼쪽 방향 화살표(←) 키를 눌렀습니다.');
        dropZone.removeChild(img);
        draggableEl.style.opacity = 1;
        draggableEl.setAttribute('tabindex', 0);
        img = null;
      }
    }

    draggableEl.addEventListener('keyup', onKeyUp);
    draggableEl.addEventListener('dragstart', onDragStart);
    draggableEl.addEventListener('dragend', onDragEnd);
    dropZone.addEventListener('dragover', onDragOver);
    dropZone.addEventListener('dragenter', onDragEnter);
    dropZone.addEventListener('dragleave', onDragLeave);
    dropZone.addEventListener('drop', onDrop);

  }

  hiddenDemo();
  dragDemo();
  ````

<br>

#### [문서 메타데이터 요소들]
  
  ```html
    <meta name="description" content="웹페이지 내용을 요약해서 기술">
    <meta name="keywords" content="웹페이지에 주요 키워드를 콤마(,)로 구분하여 작성">
    <meta name="author" content="웹페이지 제작자">
    <meta name="robots" content="index">
    <meta name="viewport" content="width="device-width, intial-scale=1"">
    <link href="default.css" rel="stylesheet" title="기본 스타일">
    <link href="fancy.css" rel="alternate stylesheet" title="팬시">
    <link href="basic.css" rel="alternate stylesheet" title="베이직"> 
    <base target="_blank" href="http://www.example.com/">
  ```

  - 메타요소는 헤더에 정의되는 문서 정보를 보여주는 요소입니다.
  - 대부분 브라우저 요소는 head를 자동으로 생성해 줍니다.
  - title Bar에서는 어떠한 태그를 쓰더라도 생략이 됩니다.
  - description, keywords, author 검색엔진 최적화 관점에서 매우 유용한 네임들 입니다.
  - viewport를 설정하지 않는다면 양쪽 여백을 자동으로 지정해줍니다. width="device-width, intial-scale=1"
  - base를 쓰게되면 기본 url주소를 설정할 수 있습니다.

  ```html
    <head> 요소
      - 문서의 제목과 스타일시트, 스크립트 링크 또는 선언을 포함하는 문서의 일반적인 정보(메타데이터)를 제공한다.
        대부분 브라우저는 마크업에서 <head> 요소가 생략될 경우, 자동으로 <head> 요소를 생성하지만 일부는 그렇지 않다.

        [자동으로 <head> 요소를 생성하지 않는 브라우저 환경]
          - Android <= 1.6
          - iPhone  <= 3.1.3
          - Opera   <= 9.27
          - Safari  <= 3.2.1.
          - Nokia 90


    <title> 요소
      - 브라우저의 타이틀 바(Title Bar)나 페이지 탭에 보여지는 문서의 제목을 정의.
        텍스트만 포함할 수 있으며 포함된 태그들은 해석되지 않음.


    <meta> 요소
      - 다른 메타 요소들(<title>, <base>, <link>, <style>)로 나타낼 수 없는 메타데이터를 정의할 때 사용.

        [메타데이터의 종류]

          - charset이 설정된 경우:
              charset 선언. 즉 웹페이지를 작성하는 일련의 형식에 사용되는 문자 인코딩(charset)에 대한 설정.
              이 속성보다 요소의 lang 속성이 우선하여 적용됨. (즉, 덮어쓰기 됨. 예: <div lang="fr">)

          - http-equiv 속성이 설정된 경우:
              pragma 지시어(Directive)로 일반적으로 웹서버가 제공하는 웹페이지가
              어떻게 제공되어야 하는지에 대한 정보를 제공.

              [예시]
                ✤ HTML 5에서는 더 이상 아래와 같이 사용되길 권장하지 않음.
                  <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
                ✤ 3초 뒤에 url 값에 설정된 페이지로 이동하게 됨.
                  <meta http-equiv="refresh" content="3;url=https://google.com">

          - name 속성이 설정된 경우:
              문서 수준 메타 데이터의 이름을 정의하며, content 속성 값을 통해 설정.

        [속성]
          - charset
          - http-equiv
          - content
              이 속성은 컨텍스트에 따라 http-equiv또는 name속성 과 연결된 값을 제공.
          - name
            - application name:
                웹 페이지에서 실행중인 웹 애플리케이션 이름 정의.
                간단한 웹 페이지는 application-name 메타를 정의해서는 안됨.
            - description
                페이지의 내용에 대한 짧고 정확한 요약을 설정.
            - keywords
                쉼표로 구분된 문자열로 페이지의 내용과 관련된 키워드를 설정.
            - author
                문서 작성자의 이름을 정의.
            - robots
                검색 로봇이 웹 페이지를 크롤링하는 동작에 대한 정의.
                  - index
                  - noindex
                  - follow
                  - nofollow
                  - noarchive
                  - nosnippet
                  - noimageindex
            - viewport
                (비표준) 초기 viewport 크기 설정에 관한 힌트를 제공.
                이 속성은 몇 개의 모바일 디바이스에 의해서만 사용됨.
                  - width
                  - height
                  - initial-scale
                  - maximum-scale
                  - minimum-scale
                  - user-scalable


    <link> 요소
      - 현재 문서와 외부 리소스와의 관계(relation)를 명시.
        이 요소는 스타일시트를 링크 하는데 가장 많이 사용됨.

        [속성]
          - rel      : 문서와의 관계 명시.
          - type     : 링크된 리소스 MIME 타입 정의. (기본 적용: text/css)
          - href     : 링크된 리소스 URL 설정.
          - hreflang : 링크된 리소스의 언어 설정.
          - media    : 링크된 리소스가 적용될 미디어(media)를 설정.

        [사용 예시]

          기본 스타일시트 설정
            <link href="style.css" rel="stylesheet">

          대체 스타일시트 설정: View > Page Style 메뉴에서 사용할 스타일시트를 고를 수 있다. (Chrome은 해당 X)
            <link href="default.css" rel="stylesheet" title="기본 스타일">
            <link href="fancy.css" rel="alternate stylesheet" title="팬시">
            <link href="basic.css" rel="alternate stylesheet" title="베이직">


    <style> 요소
      - 문서나 문서 일부에 대한 스타일 정보를 포함.
        기본적으로 CSS 언어가 사용됨.

        [속성]
          - type
          - media
          - scoped
          - title
          - disabled

        [사용 예시]

          일반적인 사용 예:
            <style type="text/css">
              body {
                color: #323232;
              }
            </style>

          scoped 속성 사용 예: ❖ 현재 제대로 지원하는 브라우저 없음.
            <section>
              <style scoped>
                p { color: #902c1f; }
              </style>
              <p> ... </p>
            </section>


    <base> 요소
      - 문서에 포함된 모든 상대 URL들의 기준 URL을 나타냄.
        한 문서에 하나의 <base> 요소만 존재해야 함.

        [사용 예시]
          <base target="_blank" href="http://www.example.com/">
  ```
</details>


## 표현 디자인(CSS)
<details id="6day">
<summary>6일차 학습</summary>


#### [CSS란?]

- css란 HTML 문서를 스타일 하는 언어를 말합니다.
- 디자인 목업 파일 스타일링 요소들을 분석하여 css 언어를 사용하여 스타일링합니다.
- sheets 문서를 style 스타일 cascading 규칙에 맞게 작성한다.
- 영상에서만 다룰 기술로 실무에서 머무르고 자신은 퇴보할 수 밖에 없기 때문에 꾸준히 어떤 정보가 올라오고 어떤 기술이 발전 됬는지 확인해야 합니다. 
www.w3.org/Style/CSS/
- 국내에서는 css 2.1버전이 가장 많이 사용되고 있습니다.
- 프론트엔드 개발자는 css를 굉장히 잘 다루셔야 합니다.
  
<br>

#### [기본 문법 & 스타일 방법]
- CSS
  ```
  선택자 {
    속성1 : 값;
    속성2 : 값2;
  }
  ```

  - 대상선택자 select
  - 블록 {}
  - 속성
  - 값
  - 속성, 값 구분 :
  - 선언문 구분 ;
  - 스타일은 헤더에서만 사용이 가능하고, body 내부에서는 사용하지 않습니다.

  - style type="text/css" 라는 mime type을 지정할 필요없이 생략한다.

  - 인라인 스타일 (inline style)
    - 요소에 직접 스타일을 추가하는 방법


  - 인터널 스타일 (internal style)
    - 헤더에 css를 style을 사용해 추가하는 방법
  - 익스터널 스타일 (external style)
    - 파일을 불러와서 사용

  ```css
  css/style.css
  select {
    color: #903000
  }
  h1 {
    color: tan
  }
  abbr {
    cursor: help; 
    text-decoration:none
  }
  ```

  ```html
  <!DOCTYPE html>
  <html lang="ko-KR">
  <head>
    <meta charset="UTF-8">
    <title>CSS 기본 문법(Syntax)</title>

    <!-- CSS 파일을 HTML 문서에 연결(External Style) -->
    <link rel="stylesheet" href="css/style.css">

    <!-- CSS 코드를 HTML 문서에 포함(Internal Style) -->

  </head>

  <body>

    <!-- 인라인 스타일: inline style -->

    <section id="about-css">
      <h1 style="">
        <dfn id="dfn-css"><abbr title="Cascading Style Sheets">CSS</abbr></dfn> 언어란?
      </h1>
      <p>
        <a href="#dfn-css">CSS</a>는 문서가 유저에게 어떻게 표시되는지를 지정하는 언어입니다. - 스타일, 레이아웃 등.
      </p>
      <p>
        문서는 보통 마크업 언어를 사용한 테스트 파일입니다. 
        — <abbr title="Hyper Text Markup Language">HTML</abbr> 이 가장 일반적인 마크업 언어이지만,
         <abbr title="Scalable Vector Graphics">SVG</abbr>나 <abbr title="eXtensible Markup Language">XML</abbr>
         과 같은 다른 마크업 언어를 만날 수도 있을 것입니다.</p>
      <p>
        사용자에게 문서를 표시한다는 것은 방문자가 이용할 수 있는 형식으로 교환하는 것을 의미합니다.
        Firefox, Chrome, Internet Explorer(IE)와 같은 웹브라우저는 문서를 컴퓨터의 화면,
        프로젝터나 프린터에서 시각적으로 표시하도록 설계되어 있습니다.
      </p>
      <figure class="figure">
        <img src="https://mdn.mozillademos.org/files/11781/rendering.svg" alt="">
        <figcaption>브라우저가 처리하는 <strong>CSS의 작동 원리</strong></figcaption>
      </figure>
    </section>

  </body>
  </html>
  ```

#### [심플 선택자]

- CSS는 HTML 요소를 선택하는데 있어 다양한 선택자 옵션을 제공합니다.
  
  - Element Type Selector
  ```
  HTMl 요소들을 직접 선택을 해서 꾸며주는 것을 말합니다.
  h1 {font-size: 100%}
  ```
  - Grouping
  ```
   그룹 선택자 // 여러개의 요소를 선택을 컴마로 그룹해 묶어주는 것을 말합니다. 
  h1, h2, h3, h4, h5, h6 {font-weight:normal}
  ```

  - Universal Select
  ```
   전체 선택자 // html 존재하는 모든 요소를 선택
   * {margin:0; padding:0}
  ```

  - Class Selector
  ```
  클래스 선택자는 .으로 구분
  멀티 선택자 클래스가 여러개 가지고 있는 클래스 선택
  p.npte.floatLeft {width : 300px}
  ```

  - Id Selector
  ```
  아이디 선택자 #으로 아이디 선택
  ul#nav {line-style:none; margin:0}
  ```

  - Descendant Selector
  ```
  자손 선택자
  p strong { font-weight:normal}
  ```

#### [속성 선택자]
  - Child Combinator
  ```
  자식 선택자 
  body > blockquote {color: #4c6a77}
  ```

  - Attribute Selector
  ```
  속성 선택자
  div[id] {font-size:11px; color:red}
  ```

  - Advanced Attribute Selector
  ```
  a[href^="http://"]
  ```

  [속성 선택자 (Attribute Selector)]
  ```
  [id]              { ... }
  [class]           { ... }
  [title]           { ... }
  [shape][title]    { ... }

  [id="about-css"]  { ... }
  #about-css        { ... }

  [class="note"]    { ... }
  .note             { ... }

  [href^="http://"] { ... }
  [src$=".svg"]     { ... }
  [src*="phone"]    { ... }
  ```

    

  [가상 클래스 (Pseudo Class)]

  ```
  :link         { ... }
  :visited      { ... }

  :hover        { ... }
  :active       { ... }

  :focus        { ... }
  :focus:hover  { ... }
  :focus:active { ... }

  :first-child  { ... }
  :last-child   { ... }
  :nth-child(n) { ... }

  :lang(ko)     { ... }
  ```
    


  [가상 요소 (Pseudo Element)]
  ```
  ::first-letter { ... }
  ::first-line   { ... }
  ::before       { ... }
  ::after        { ... }
  ```
   


  ```css
  /* body 요소 내부의 모든 자손 선택 */
  body * {}

  /* body 요소 내부의 모든 자식(child) 선택 */
  body > * {
    outline : 3px solid #fc414b;
  }

  /* 속성선택자 *.
  [title][lang] { }'
  '
  /* [id="about-css"] { outline: 3px solid #fc414b; } */
  /* #about-css {outline: 3px solid #fc414b} */

  /* [class="note box"] { outline: 3px solid #fc414b}
  .box { }
  .note { }

  {title^="Scalable"} { outline: 3px solid #fc414b; }
  ```
#### [가상 클래스 선택자]
- Link Pseudo-class

  ```css
  a:link, a:visited {color:#999}
  a:hover, a:active {color:#333} // 마우스로 클릭 했을때 그 당시 css
  p:hover {color:#78757e}

  input:focus {background:#e3e2e8}
  input:focus:hover {background:#ced132}

  ** href에만 적용
  a:link {
    color: #ff487c;
  }
  a:visited {
    color: #32c29a;
  }

  h1, h2, p {
    color: #777;
  }

  h1:hover,
  h2:hover,
  p:hover {
    color: #222;
  }

  p:active {
    background: #ff0;
  }

  focus는 키보드 접근이 가능한 요소에게 줘야 합니다.
  미국 같은 경우에는 법률 조항이 업격합니다. (접근성을 엄청나게 강조함.)
  a:focus {
    outline-offset: 3px;
    outline: 3px solid #333;
  }

  a:focus:active {
    outline: none;
    background-color: #fe8440;
  }

  /* link-list li:first-child */
  .link-list li:nth-child(odd) {
    outline: 3px solid #ff0;
  }

  /* link-list li:last-child */
  .link-list li:nth-child(even) {
    outline: 3px solid #4ec13f;
  }

  :lang(en) {
    font-family: "Times New Roman";
  }

  :lang(ko-KR) {
    font-family: "Spoqa Han Sans";
  }
  ```

  ```html
  <section id="css-reference">
    <h2>CSS 레퍼런스</h2>
    <ul class="link-list">
      <li>
        <a href=":link">:link</a>
      </li>
      <li>
        <a href=":visited">:visited</a>
      </li>
      <li>
        <a href=":hover">:hover</a>
      </li>
      <li>
        <a href=":active">:active</a>
      </li>
    </ul>
  </section>

  :first_child {...}  // 첫번째 자식
  :last_child {...}   // 두번째 자식
  :nth-chold(n)       // n번째 자식

  :lang(ko)           // HTMl 사용 되는 언어에 따라 디자인을 적용해 줄 수있습니다.
  ```

  ```html
  <section id="about-css">
    <h1>
      <dfn id="dfn-css"><abbr lang="en" title="Cascading Style Sheets">CSS</abbr></dfn> 언어란?
    </h1>
    <p class="note">
      <a lang="en" href="#dfn-css">CSS</a>는 문서가 유저에게 어떻게 표시되는지를 지정하는 언어입니다. 
      - 스타일, 레이아웃 등.
    </p>
    <p class="note box">
      문서는 보통 마크업 언어를 사용한 테스트 파일입니다. — <abbr lang="en" title="Hyper 
      Text Markup Language">HTML</abbr> 이 가장 일반적인 마크업 언어이지만, <abbr lang="en" title="Scalable Vector 
      Graphics">SVG</abbr>나 <abbr lang="en" title="eXtensible Markup Language">XML</abbr>과 같은 다른 마크업 언어를 
      만날 수도 있을 것입니다.</p>
    <p>
      사용자에게 문서를 표시한다는 것은 방문자가 이용할 수 있는 형식으로 교환하는 것을 의미합니다.
      Firefox, Chrome, Internet Explorer(IE)와 같은 웹브라우저는 문서를 컴퓨터의 화면,
      프로젝터나 프린터에서 시각적으로 표시하도록 설계되어 있습니다.
    </p>
    <figure class="figure">
      <img src="https://mdn.mozillademos.org/files/11781/rendering.svg" alt="" width="678" height="261.58">
      <figcaption>브라우저가 처리하는 <strong>CSS의 작동 원리</strong></figcaption>
    </figure>
  </section>
  ```

#### [가상 요소 선택자]
- 가상요소와 가상 클래스
```
: 가 하나면 가상 클래스 요소이고 ::면 가상 요소 입니다. 
항상 코딩 할때 생각 했었는데 어쩔때는 한개고 어쩔때는 두개여서 하나만 써도 적용이 되서 하나만 써왔습니다.

가상 클래스 요소와 가상 요소를 구분하기 위해서 사용 해야한다. 하나만 써도 두개를 써도 하위호환을 위해 적용이 된다.
```

-
```
/* 첫번째 글자 수정 */
p::first-letter {
  font-weight: bold;
  font-size: 20px;
}

#dfn-css::before {
  content: '[';
  font-style: normal;
}

#dfn-css::after {
  content: ']';
  font-style: normal;
}

figure::before {
  content: 'Figure';
  display: block;
  margin-bottom: 10px;
  border-radius: 4px;
  padding: 0.3em 0.8em;
  background: #222;
  color: #fff;
}

::first-line => 요소의 첫번째 줄을 선택하는 가상 요소
```

</details>

<details id="7day">
<summary>7일차 학습</summary>

#### [상속]  
- 상속이란 물려 받는 것을 말합니다.
  ```
  상속이 되는 속성 (글자색, 글자 디자인에 관련된 것)
    - color
    - font-size
    - font-family
    - letter-spacing // 자간
  ```
  
  ```
  상속이 되지 않는 속성 (공간에 관련된 것)
  - outline
  - margin
  - border
  - padding
  ```

  ```
  css/inheit.css

  article {
    color: #fe4940;
    font-size: 22px;
    font-family: Arial;
    letter-spacing: -0.5px;
    padding: 20px;
  }
  ```

  css를 확인할 때 상속받지 않는 다면 해당 속성은 불투명하게 된다.

  ```
   <section id="css-inheritance">

    <h1>
      <abbr title="Cascading Style Sheets">CSS</abbr> 상속
    </h1>

    <article class="part">
      <h2>상속되는 속성</h2>
      <p>요소의 <strong>상속되는 속성</strong>에 값이 지정되지 않은 경우, 요소
      는 부모 요소의 해당 속성의 계산 값을 얻습니다. 
      오직 문서의 루트 요소만 속성의 요약절에 주어진 초기 값을 얻습니다.</p>
      <p>상속되는 속성의 대표적인 예는 color 속성입니다.</p>
      <p><abbr>CSS</abbr> 스타일 규칙:</p>
      <div class="code-block"><pre>
<span class="selector">p</span> <span class="brace">{</span>
  <span class="property">color</span>: <span class="value">green</span>;
<span class="brace">}</span>
</pre></div>
      <p><abbr title="Hyper Text Markup Language">HTML</abbr> 마크업:</p>
      <div class="code-block"><pre><span class="tag">&lt;p&gt;</span>이 단락은 <span class="tag">&lt;em&gt;</span>강조된 
      텍스트<span class="tag">&lt;/em&gt;</span>를 포함하고 있습니다.<span class="tag">&lt;/p&gt;</span></pre></div>
      <p>
        <code>em</code> 요소는 <code>p</code> 요소로 부터 <code>color</code> 속성 값을 상속했기 때문에, <strong>"강조된 텍스트"
        </strong>는 녹색으로 보입니다. 속성의 초기값을 얻지 않습니다.
      </p>
    </article>

    <article class="part">
      <h2>상속되지 않는 속성</h2>
      <p>요소의 <strong>상속되지 않는 속성</strong>에 어떤 값이 지정되지 않는 경우, 요소는 그 속성의 초기 값을 얻습니다.</p>

      <p>상속되지 않는 속성의 대표적인 예는 <code>border</code> 속성입니다.</p>

      <p><abbr>CSS</abbr> 스타일 규칙:</p>

<div class="code-block"><pre>
<span class="selector">p</span> <span class="brace">{</span>
  <span class="property">border</span>: <span class="value">3px solid #333</span>;
<span class="brace">}</span></pre></div>

      <p><abbr title="Hyper Text Markup Language">HTML</abbr> 마크업:</p>

      <div class="code-block"><pre><span class="tag">&lt;p&gt;</span>이 단락은 <span class="tag">
      &lt;em&gt;</span>강조된 텍스트
      <span class="tag">&lt;/em&gt;</span>를 포함하고 있습니다.<span class="tag">&lt;/p&gt;</span></pre></div>

      "<strong>emphasized text</strong>"는 테두리가 없습니다 (<code>border-style</code>의 초기 값이 <code>none</code>
        이기 때문입니다).
    </article>

  </section>
  ```

#### [우선 적용 규칙] 

캐스케이딩 
```
여러 스타일 시트를 결합하고 이들 사이에서 충돌나지 않고 css를 적용하는 프로세스.
```

```
/*
  ------------------------------------------------
  CSS 캐스케이드 (Cascade)
  ------------------------------------------------

  cascading:

    The process of combining several style sheets
    and resolving conflicts between them.

    Håkon Wium Lie (CSS 공동 창시자)는 CSS에 관한
    PHD 논문에서 "여러 스타일 시트를 결합하고 이들 사이의
    충돌을 해결하는 프로세스"라는 용어로 "Cascade"를
    말하고 있습니다.

    https://www.wiumlie.no/2006/phd/

  CSS(Cascading Style Sheets )는 캐스케이드 개념이
  중요하다는 것을 약어에서 강조. 가장 기본적인 수준에서는
  규칙 순서가 중요하지만 그보다 더 복잡하다는 것을 말한다.

    1. 중요성 (Importance)
       !important 선언은 다른 모든 선언보다 우선권을 가진다.

      [NOTE]
      !important가 적용된 속성을 덮어 쓰려면, 다시 !important를
      사용해야 하기에 최대한(절대!!) 사용하지 않도록 노력해야 한다.

    2. 특성 (Specificity)
       선택자의 우선권에 대한 척도.
       각 척도를 1, 10, 100, 1000 단위로
       생각하면 이해하기 좋다.


       요소 선택자 < 클래스 선택자 < ID 선택자 < 인라인 스타일
       0,0,0,1    0,0,1,0      0,1,0,0   1,0,0,0

      [NOTE]
        *, >, +, ~ 등 콤비네이터(Combinators),
        :not() 가상 클래스는 특성에 영향을 주지 않는다.

      [예시]
        *                         -- 0000
        a                         -- 0001
        .link                     -- 0010
        a[href]                   -- 0011
        li:nth-child(2) a:hover   -- 0022
        .nav:nth-child(2) a:hover -- 0031
        #outer a                  -- 0101
        #outer #inner a           -- 0201
        style="color: tan"        -- 1000
                                  -- !important

    3. 소스 순서
      중요성, 특성이 설정되지 않았거나 동일한 경우
      나중에 나온 소스의 스타일이 우선권을 가진다.

      [예시]
        p { color: #930212; }
        p { color: #d5727e; } // 우선권을 가진다.

  참고: https://goo.gl/BAhjiN

*/
```

```
/* 0011 */
li:nth-child(2) {
  outline: 4px solid #ff0 !important;
}

/* 0012 */
ul li:nth-child(2) {
  outline-width: 1px;
  outline-color: #b11a25;
}

ul.cascading-rules li:nth-child(2) {
  outline-width: 10px;
  outline-color: #eec129;
  outline-style: double;
}
```

#### [타이포 그래피]  
```
/*
  ------------------------------------------------
  CSS 타이포그래피 (Typography)
  ------------------------------------------------

  폰트(Fonts) 스타일 속성
    - 폰트에 영향을 주는 속성으로
      적용되는 모양, 크기, 굵기, 기울임 등.

      font-family
      font-size
      font-weight
      font-style
      font-variant

      ※ 글자 색상은 color 속성으로 설정.
        color keywords: red, gree, blue, pink, black
        hex color code: #RRGGBB / 0 ~ 9, a ~ f 예) #1868a7
        rgb, rgba: RED, GREEN, BLUE, ALPHA 예) rgba(127,255,0,0.3)
        hsl, hsla: HUE, SATURATION, LIGHTNESS, ALPHA 예) hsla(360,60%,70%,1)
      ※ 웹브라우저는 운영체제가 지원하는 기본 폰트(웹 안전 폰트)만
        화면에 렌더링 한다. (참고: cssfontstack.com)
        즉, 사용된 폰트가 사용자 컴퓨터에 없으면 렌더링 X.

        웹 안전 폰트
        Arial            [sans-serif]  고딕체
        Verdana          [sans-serif]  고딕체
        Courier New      [monospace]   코드체(공간이 동일)
        Georgia          [serif]       명조체
        Times New Roman  [serif]       명조체
        Trebuchet MS     [serif]       명조체

        하지만 웹 안전 폰트만으로 디자인 하는 디자이너는 없다!
        Helvetica는 디자이너가 애용하는 폰트이지만...
        Windows는 기본 지원하지 않는다. (Mac OSX는 지원)

      ※ 비주얼 디자인 과정에서 적용 가능한 웹폰트를 사용해야 한다.
        폰트 저작권에 주의! (참고: hyundaicard.com)

      ※ 저작권 걱정 없는 폰트
        fonts.google.com
        google.co.kr/search?q=무료+웹폰트

  --------------------------------------------------

  텍스트(Text) 레이아웃 속성
    - 텍스트 간격 및 레이아웃 기능에 영향을 주는 속성으로
      행간, 자간, 어간, 정렬, 변형, 꾸밈, 그림자

      line-height

      letter-spacing
      word-spacing

      text-align
      text-indent
      text-transform
      text-decoration
      text-shadow

      white-space
      word-break
      word-wrap

*/
```

```css
@font-face {
  font-faily: IropkeBatangM;
  src: local(IropkeBatangM).
      url(IropkeBatangM.eot?#iefix) format('embedded-opentype'), url(IropkeBatangM.woff) format('worf');

  /* 사용할 유니코드의 범위를 정함. 유니코드 범위 내 사용하는 문자가 없으면 웹폰트를 다운로드 안함.
  unicode-range: U+0-10FFFF;
}
```

```css
css/typography.css
body {
  font-family: IropkeBatangM;
  font-size: 16px;
  line-height: 1.5;
  color: #483372;
}

h1 {
  font-size: 32px;
  font-style: italic;
  font-weight:normal;
  /* text-transform: lowercase; */
  /* text-veriant: all-small-caps; */
  /* text-decoration: overline underline line-through; */
  /* text-shadow: -5px -5px 3px #9bdbde;
                   5px  5px 3px #943978 */
}

p {
  letter-spacing: 0;
  font-size: 14px;
  word-spacing: 0.02em /* 글자 간격 */
}

.white-space-ex {
  white-space: pre;
  white-space: nowrap;
  white-space: nowrap;
}

.word-break-ex {
  /*
    단어의 분리를 어떻게 할 것인지 결정

    (공백/뛰어쓰기) 수고했어. 오늘도
    (음절)         수 . 고 . 했 . 어 . 오 . 늘 . 도
   */

   /* word-break: break-all */

   /*
    박스의 가로 영역에 넘친 단어 내에서
    임의의 분리 여부를 결정하여 줄바꿈 관여
   */

   word-wrap: break-word;
}

```

```html
<!DOCTYPE html>
<html lang="ko-KR">
<head>
  <meta charset="UTF-8">
  <title>CSS 타이포그래피(Typography)</title>
  <!-- 웹 폰트 로드 -->
  <link
    rel="stylesheet"
    href="fonts/webfonts.css"
    media="none"
    onload="if(media!='all')media='all'">
  <link rel="stylesheet" href="css/style.css">
  <link rel="stylesheet" href="css/typography.css">
</head>

<body>

  <div class="album">
    <img
      src="images/Dalmoon_28.jpg"
      alt="옥상달빛 28"
      width="240" height="240">
    <audio
      src="media/Thanks-today.mp3"
      preload controls autoplay></audio>
  </div>

  <section id="css-typography">

    <h1>수고했어. 오늘도.</h1>
    <!-- <h1 lang="en">Thanks. Today.</h1> -->

    <p>세상 사람들 모두 정답을 알긴 할까<br>
      힘든 일은 왜 한번에 일어날까</p>

    <p>나에게 실망한 하루!<br>
      눈물이 보이기 싫어<br>
      의미 없이 밤 하늘만 바라봐</p>

    <p>작게 열어둔 문틈 사이로<br>
      슬픔 보다 더 큰 외로움이 다가와 더 날</p>

    <p>수고했어 오늘도<br>
      아무도 너의 슬픔에 관심 없대도<br>
      난 늘 응원해, 수고했어 오늘도</p>

    <p>빛이 있다고 분명 있다고 믿었던<br>
      길마저 흐릿해져 점점 더 날</p>

    <p>수고했어 오늘도<br>
      아무도 너의 슬픔에 관심 없대도<br>
      난 늘 응원해, 수고했어 수고했어 수고했어 오늘도</p>

    <p>라랄라라라라라 라라라 라라라라라라라라<br>
      라라 라라라라 라라라 라라라</p>

    <p>수고했어 오늘도<br>
      아무도 너의 슬픔에 관심 없대도<br>
      난 늘 응원해, 수고했어 오늘도</p>

    <p class="white-space-ex" hidden>
      세상 사람들 모두 정답을 알긴 할까
      힘든 일은 왜 한번에 일어날까

            나에게 실망한 하루!
      눈물이 보이기 싫어
      의미 없이 밤 하늘만 바라봐

      작게 열어둔 문틈 사이로
      슬픔 보다 더 큰 외로움이 다가와 더 날

      수고했어 오늘도
      아무도 너의 슬픔에 관심 없대도
      난 늘 응원해, 수고했어 오늘도

      빛이 있다고 분명 있다고 믿었던
      길마저 흐릿해져 점점 더 날

      수고했어 오늘도
      아무도 너의 슬픔에 관심 없대도
      난 늘 응원해, 수고했어 수고했어 수고했어 오늘도

      라랄라라라라라 라라라 라라라라라라라라
      라라 라라라라 라라라 라라라

      수고했어 오늘도
      아무도 너의 슬픔에 관심 없대도
      난 늘 응원해, 수고했어 오늘도
    </p>

    <div class="word-break-ex lone-url" hidden>

      https://longurlmaker.com/go?id=z4Is.gd8c11rangy50farawayRedirx1drawn%2Bout60c3protractedTinyLinkstringylinger
      ingfar%2BreachinglMyURLSHurl86018lengthy7frunningoutstretched1111ilengthy2xSimURLSmallr800xSimURL361juEasyURL
      SimURL0022faraway1095xhighfar%2Boff1618sustained0Shima8961toutstretchedexpanded0stretch611220drawn%2BoutdwkT
      ghtURL8kDoioplongish10Xil14b101ShredURLTraceURLbptoweringB6512TinyURL6towering0rGetShorty004bm5301URLprotrac
      ted0prolonged61MooURLy1948jspread%2Bout428u0t3stretchingfarawaylasting11ShredURLc2bDigBigexpandedX.se90a20Ti
      nyURL26WapURLr1cprolongedkelongatedc1f2c01loftylengthycontinuede7WapURLgGetShorty2NutshellURLcontinued6a2la
      stingr5protracted1expandeddistantspread%2BoutURl.iersustainedNotLongSHurl3w2SimURL011xSnipURL02GetShorty2prol
      onged0f02f60blingeringIs.gd
      301URLTinyLinktowering3d200t01osustained2WapURL90ShortURL11spread%2Boute02URLPieFly2toweringDwarfurl70elong
      ated9s070SnipURL6Is.gd7spread%2Boutc0hy210vtcnf43Redirxb9148n1lingering6PiURL16URLcutaspread%2BoutYATUCouts
      tretchede70lUlimita1e610ShortenURL1lnk.inenduringUlimit0U760l8m72011793v7020TightURLelongatedYATUCt6UrlTeae
      tc91e5kspun%2Bout010d1e1b1Dwarfurl6Shortlinksb0sustained0enlarged6great1187e5e690URLCutter1spun%2Bout10draw
      n%2Bouttall4EasyURLDecentURLenduringd1eTraceURL5yGetShortyTinyLinkfar%2Boff1prolonged4cc0stretcheddeepprotr
      acted3f001elongate9018ystretc
      hinglastingi7TinyURL7expanded910continuedremotef8sustainedz175lingeringcbloftyprolonged10079running0UlimitB
      6515Shrinkr00LiteURL1loftyoutstretchedclnk.in3farawayg5runningTinyLinkspread%2Bout1stringy11c036greatfarawa
      ystretchingefar%2Boff31spread%2Bout4kDoiopMooURL53m19Beam.tolastingShredURL1s25ShimBeam.to8nstretchtowering
      80StartURLShortURL4lengthened018Is.gdNotLongzWapURLNutshellURLe2spun%2Bout119elongated7elongated5outstretch
      edh8k1stringyloftyShredURL84
      running06308d071Minilien3wg3UrlTealoftystretchedwCanURLfar%2Boff7atf104083towering820ganglingw35m1a063LiteU
      RLt081NanoRef361lnk.in0deep0Shrinkr6e80far%2Boff9170Redirxy6btspread%2Boutsustained10UlimitShortlinks2tower
      ingGetShorty3ShrinkrDecentURLsustaineddbg1nfShortURL331a001enlargedB65RedirxelongatedMinilien809UrlT
    </div>

  </section>

<script>
  document.querySelector('audio').volume = 0.5;
</script>
</body>
</html>
```



</details>

<details id="8day">
<summary>8일차 학습</summary>

#### [박스 모델]    

- CSS 사용해서 레이아웃을 조작할껀데 레이아웃을 조작하기 위해서 박스 모델을 이해해야 합니다.
block inline

HTML5에서는 flow contents(block) 요소 와 Phrasing Contents(inline) 요소라고 합니다.

블록 박스는 다른 박스에 포함되거나, 포함할 수 있고, 너비(width) / 높이(height) 설정이 가능합니다. 내부에 콘텐츠를 포함하지 않을 경우 높이는 0 입니다.

인라인 박스는 블록 요소는 포함 할수 없습니다. 그리고 공간이 없습니다. 너비(width)와 높이(height) 설정이 불가능 합니다. (내부 컨텐츠 만큼 높이와 너비를 가지게 됩니다.)

인라인 블록 박스는 기본적으로 인라인퍼럼 표시가 되지만 블록박스처럼 너비(width)와 높이(height) 설정이 가능합니다.

중요. 인라인 요소지만 가로와 높이 설정이 가능합니다. 인라인 블록 박스는 안에 있는 단어들을 한 묶음으로 보기 때문에 범위를 벗어나면 전체가 개행이 됩니다.


  ```
   ------------------------------------------------
    CSS 박스 모델 (Box Model)
    ------------------------------------------------

    CSS를 사용해 HTML 요소를 레이아웃(배치) 하려면 박스 모델에
    대해 먼저 이해해야 한다. 암기할 필요는 없고 쓰다보면 자연적으로 외워지게 됩니다.

      [BLOCK vs INLINE]
        * block level 요소 (Flow Contents)
        * inline 요소 (Phrasing Contents)

        [block 요소들]
          - address
          - article
          - aside
          - audio
          - blockquote
          - canvas
          - dd
          - div
          - dl
          - fieldset
          - figcaption
          - figure
          - footer
          - form
          - h1~6
          - header
          - hr
          - noscript
          - ol
          - output
          - p
          - pre
          - section
          - table
          - tfoot
          - ul
          - video
  ```

  content, padding, border 박스와 다르게 margin는 색깔을 줄수없습니다. 
  인라인 박스인 경우 좌/우 방향으로 마진과 패딩을 설정할 수 있지만 상/하 방향으로는 공간이 설정 되지 않습니다.
  마진 박스인 경우 음수 값을 쓸 수 있지만 패딩과 테두리 박스는 음수 값을 줄 수 없습니다.
  인라인 박스는 padding으로 가로를 줄 수 있습니다. 하지만 세로를 할 경우 세로의 공간이 벌어지진 않지만 해당 영역에 대해 css를 줄 수 있습니다.

  4개의 값을 주면 패딩과 마진을 줄때 시계 방향으로 크기가 할당 됩니다.
  top, right, bottom, left

  패딩과 마진을 3개의 인자만 줘도 왼쪽값은 상속 받게 됩니다. 
  top, right, bottom

  가운데 정렬 -> width와 line-height를 동일하게 주면 버티컬이 가운데에 정렬이 됩니다.


  ```
  [BOX]
        * margin-box   --  외부 공간 박스
        * border-box   --  테두리 공간 박스
        * padding-box  --  내부 공간 박스
        * content-box  --  콘텐츠 공간 박스

        [margin]
          * margin-top
          * margin-right
          * margin-bottom
          * margin-left
          * margin: t r b l
          * margin: t r b (l=r)
          * margin: t r (b=t) (l=r)
          * margin: t (r=t) (b=t) (l=r)

        [border]
          * border-(top|right|bottom|left)-width
          * border-(top|right|bottom|left)-style
          * border-(top|right|bottom|left)-color
          * border: width style color
          * border-top: width style color
          * border-right: width style color
          * border-bottom: width style color
          * border-left: width style color

        [padding]
          * padding-top
          * padding-right
          * padding-bottom
          * padding-left
          * padding: t r b l
          * padding: t r b (l=r)
          * padding: t r (b=t) (l=r)
          * padding: t (r=t) (b=t) (l=r)
  ``` 
  
  textarea인 경우 최대값과 최소값을 설정할 수 있습니다.

  글자를 넣고 1em을 넣게되면 글자수 만큼 패딩이 늘어납니다.

  ```
      [DIMENSION]
        * width       --  박스 너비
        * height      --  박스 높이
        * min-width   --  박스 최소 너비
        * min-height  --  박스 최소 높이
        * max-width   --  박스 최대 너비
        * max-height  --  박스 최대 높이
```
 box sizeing 박스 사이즈 설정 방법.

```
      [BOX SIZING]
        * content-box
        * border-box

        - content-box (default):
          width = content-box
          height = content-box

        - border-box:
          width = content-box + padding-box + border-box
          height = content-box + padding-box + border-box

  ```
 박스를 넘쳐났을 떄 처리방법.

  ```
      [FLOW]
        * overflow  --  박스를 넘쳐난 상태(흐름) 조정
          - auto    -- 자식이 부모이상 넘치게 되면 스크롤이 생깁니다.
          - visible -- 전부 보여줍니다.
          - hidden  -- 자식이 더 있어도 스크롤이 생략됩니다. X, Y
          - scroll  -- 스크롤이 생깁니다.
  ```



#### [리스트 스타일링]    
같은 속성일 경우 나중에 있는 css가 먼저 적용 된다.

```
:root {
  font-size:10px;
}

body {
  font-size: 16px;
  font-size: 16rem;
}

rem => root em, 루트 기본 값으 1.6배가 됩니다.

```

리스트 블릿을 list-style-type을 사용하면 다른 타입으로 바꿀 수 있습니다.

```
ul {
  /*
  list-style-type: none; -- ul 초기화
  padding-left: 0; */    -- ul에 의한 패딩 초기화  
  margin:0;
  list-style-image: url("../images/start.svg") -- ul 아이콘 이미지로 변경
  /* list-style-type: decimal-leading-zero; */
  /* list-style-position: inside; */
  /* margin-top: 0;
  margin-bottom: 0; */
}

line-style: square url("star.svg") inside(속기 유형 작성법)

```

#### [배경 스타일링]   

```
body {
  background-image:url("../images/model.jpg");
  background-repeat: no-repat; repat-x; repat-y;
  background-position: 좌우 상하
  background-attachment: fixed;
  background: 4가지
  background-size:좌우 상하
}

#css-background {

}

.bg-image {
  background-color: #000999;
  background-image: url("../images/NewYork-US.jpg") no-repeat center -60px;
  background-position: 좌우 상하
  background-size: contain;
  background-size:cover;

}

.is-floral {
  background: url("../images/oriental-floral-patten.svg") center;
  background-size: 150px;
}

.is-model {
  background: url("../images/model.jgp") center
}

.background-clip {
  box-sizing: border-box;
  border: 20px solid rgba(0,0,0,0,2);
  padding: 20px;
  background: url("../images/model.jpg") center;
  background-size: contain;
  background-clip: border-box;
  background-clip: padding-box
}
```
```
배경 색: background-color
배경 이미지: background-image
배경 위치: background-position
배경 고정: background-attachment
배경 반복: background-repeat
배경 크기: background-size
배경 기준: background-origin
배경 클리핑: background-clip
```

</details>

<details id="9day">
<summary>9일차 학습</summary>

#### [플로팅 레이아웃]    
뷰포트와 관련하여 박스를 레이아웃 하는 방법

- 일반적인 레이아웃 흐름(Normal Layout Flow)
```
HTML이 기본적으로 화면에 랜더링하는 것을 말합니다. 마크업 순서대로 위에서부터 아래 방향으로 나열 됩니다.
```
- 플로팅(Floating) 레이아웃
```
일반적으로 레이아웃은 위에서 아래로 쌓이지만 floating은 왼쪽 오른쪽으로 부유 시킬 수 있습니다.
이미지에 텍스트를 둘러싸기 위해 만든 레이아웃입니다.
float 기본 속성은 none입니다.
컬럼을 나눠서 컬럼 레이아웃 디자인을 손쉽게 구현할 수 있습니다.
float으로만 만들어진 요소로만 자식을 가지고 있을 때 세로의 길이는 0 입니다.

클리어 라는 요소 검색해서 알아보기.

float 초기화 clear
그리고 float 양쪽을 클리어 하고 싶다면 clear:both를 사용하면 됩니다. 
하지만 지금 시대는 쓰면 안되고 원리를 이해하기 위해 썼습니다.
```

첫번쨰 방법 (권장x)
```
.clear {
  clear: left;
}
```

두번째 방법 (권장x)
```
box-group {
  overflow: auto;
  margin-top: 20px;
  border: 10px solid #e9e9e9
}

.box {
  margin: 0;
  margin-left: 10px;
  margin-right: 10px;
  width: 140px;
  height: 140px;
}
```

세번째 방법 (주사용) 
```
.clearfix:after {
  content: "after content";
  display: block;
  clear: both;
  visabllity: hidden;
  height: 0px;
}

.clearfix:after {
  content: "";
  display: block;
  clear: both;
  visabllity: hidden;
  height: 0px;
}
```

실습
```
.magazine * {
  margin: 0;
}

.magazine {
  height: 100%;
  width: 1400px;
  margin-left: auto;
  /* background: cprazon-salvaje.jpg */
  background: url("../images/corazon-salvaje.jpg") no-repeat right bottom;
}

.is-contents p {
  margin-bottom: 21px;
}

/*
.is-contents p:nth-of-type(2) {
  padding-left: 200px;
}
*/

.side-layout {
  font-size: 500px;
  line-height: 0;
  float: left;
  margin-left: -230px;
}
```

플로트를 사용하면 잡지와 같은 디자인이 가능합니다.

#### [포지셔닝 레이아웃]    
포지셔닝은 웹브라우저가 랜더링하는 기본 레이아웃 흐름(Normal Layout Flow)을 재정의하여 흥미로운 효과를 낼때 사용합니다.

- 상대적인 위치 설정* relative
```
.is-blue {
  position: relative;
  top: 30px;
  right: -100px;
  z-index:1; -- 더 높을 수록 상위에 있다.
}

.is-yellow {
  position: relative;
  top: 30px;
  left: 40px;
  z-index:3;
}

.is-green {
  position: relative;
  bottom: 300px;
  left: 120px;
  z-index: 1;
}

```
- 절대적인 위치 설정 
  - absolute를 쓰게 되면 밑에 있는 요소들이 위로 올라올려는 성질 떄문에 relative를 같이 사용해야 합니다.
```
.is-yellow {
  position: absolute;
  z-index: 100;
  top: 20px;
  right: 20px;
  /* z-index: 100; */
}
```

- 페이지의 스크롤과 상관없이 항상 브라우저 창의 동일한 위치에 차지한 UI요소를 만들고자 한다면 포지셔닝을 사용합니다.

- 고정적인 위치 설정
위에서 값이 있다면 initial로 초기화 시킬 수 있다.

.is-yellow {
  position: fixed;
  top: initial;
  left: 0;
  bottom: 0;
}

</details>

<details id="10day">
<summary>10일차 학습</summary>

#### [테이블 스타일링]  
- HTML 요소에 border라는 것을 사용하면 안됩니다. 그것은 css에서 처리하기 때문입니다.
- 디자이너가 테이블 디자인을 할때 테이블의 접근성으 고려하지 않습니다.
- 디자인 상에 없다고 해도 모든 사용자를 고려하여 테이블 요약 내용을 구조화해야됩니다.

```css
재사용 가능한 클래스를 만들어서 숨겨야한다. 화면에서는 감쳐지지만 화면에서는 읽어집니다. width와 height가 0이면 화면에서 없다고 처리해서 1px을 써야합니다. 그리고 화면에서 안보이게 하기 위해 clip을 0으로 만들어줍니다.

/* 접근성(accessibility, a11y)을 고려한 화면 감춤 */
.a11y-hidden {
  overflow: hidden;
  position: absolute;
  clip:     rect(0,0,0,0);
  width:    1px;
  height:   1px;
  margin:   -1px;
  border:   0;
  padding:  0;
}

캡션인 경우에 해당 클래스가 들어가게 되면 1px정도 칸이 생깁니다. 
그래서 static으로 초기화 시켜줘야합니다.
/* 화면에 표시되는 caption 요소의 공간 제거를 위한 설정 */
caption.a11y-hidden {
  position: static;
}

table, th, td {
  /* [1] 테이블, 제목/내용 셀 테두리 표시 설정. */
  border: 1px solid #212121;
}

table {
  /* [2] 테이블 셀 사이 간격을 접음. */
  border-collapse: collapse;
  /* [3] 테이블 보더 사이 간격 설정 separate 설정 필요하다.*/
  border-spacing: 10px;
  /* [4] 캡션 위치 설정 (top | bottom) */
  caption-side: bottom;
  /* [5] 테이블 레이아웃 설정 기본값 auto 자동으로 늘어남 */
  table-layout: fixed;
}

th, td {
  /* [6] 테이블 셀은 마진이 설정되지 않음 */
  margin: 10px;
  /* [7] 테이블 셀은 패딩은 설정가능 */
  padding: 0.4em 0.6em;
  /* 빈셀의 표시 설정 */
  empty-cells : hide;
}

<p id="kakaobank-notice-summary" class="a11y-hidden">
  카카오 뱅크의 공지사항을 안내하는 표입니다.
</p>
aria0describedby="kakaobank-notice-summary"

걉션 경우 빈칸이 생기기때문에 static을 줘야한다.

/* 실습 */

/**
 * --------------------------------
 * 테이블 디자인
 * ----------------------------- */

/* 테이블 캡션 */
#notice-table caption {
  text-align: left;
  font-size: 22px;
  margin-top: 30px;
  margin-bottom: 20px;
}


/* 테이블, 셀 공통 설정 */
#notice-table, #notice-table th, #notice-table td {
  border-top: collapse;
}


/* 테이블 설정 */
#notice-table {
  width: 100%;
  border-top: 1px solid #d0d0d0;
  border-collapse: collapse; -- 셀 간격이 사라짐
  /* border-spacing: 20px 10px; */ -- 셀 간격을 설정할 수 있음.
}

#notice-table.is-zebra tr:nth-child(even) {
  background: #e5e5e5;
}


/* 제목,내용 셀 설정 */
#notice-table th, #notice-table td {
  border-bottom: 1px solid #d0d0d0;
  padding: 0.55em 0.8em;
  font-size: 14px;
}

#notice-table th {
  border-bottom: none;
  background: #f4f4f4;
  color: #828282;
  font-weight: normal;
}

#notice-table col:nth-child(1) { width: 70px; }
#notice-table col:nth-child(3) { width: 115px; }

/* 제목, 내용 셀 설정 */
#notice-table th, #notice-table td {
  border-bottom: 1px solid #d0d0d0;
  padding: 0.55em 0.8em;
}

#notice-table.is-zebra tr:hover {
  background: #ababab;
}

#notice-table th {
  background: #f4f4f4;
  color: #828282;
  font-weight: normal;
}

#notice-table td:not(:nth-child(2)) {
  text-align: center;
  color: #909090
}

#notice-table a {
  color: #828282;
  text-decoration: none;
}

#notice-table a:hover,
#notice-table a:focus {
  text-decoration: underline;
  /* 
    padding-bottom: 2px;
    border-bottom: 1px solid currentColor;
  */
}


```

#### [폼 스타일링]  

- 폼 컨트롤 가상 클래스(Pseudo Classes) IE 9+ 부터 지원
```
- input:radio, input:checkbox, option 컨트롤 체크 상태 표시
:checked

- 활성화된 컨트롤 상태 표시
:enabled

- 비활성화된 컨트롤 상태 표시
:disabled

- 불확실한(indeterminate) 상태의 컨트롤 표시
:indeterminate

- 필수(required) input, textarea, select 컨트롤의 상태 표시
:required

- 선택(optional) input, textarea, select 컨트롤의 상태 표시
:optional

- 유효(valid)한 input, form 컨트롤의 상태 표시
:valid

- 유효하지 않은(invalid) input, form 컨트롤의 상태 표시
:invalid

- button, input:checkbox, input:radio, option 컨트롤 기본 상태 표시
:default

- min, max 값을 가지는 input 컨트롤의 허용 범위(in range) 상태 표시
:in-range

- min, max 값을 가지는 input 컨트롤의 비허용 범위(out of range) 상태 표시
:out-of-range

- 읽기만 가능한 input, textarea의 상태 표시 
:read-only

- 읽기 쓰기 가능한 input, textarea의 상태 표시
:read-write
```

실습 
```
라벨같은 경우 두번 클릭했을시 드래그가 됩니다. user-select: none;을 사용해 막아줍니다.
.modal-form label {
  user-select: none;
}

.modal-form input {
  width: 100%;
  border: none;
  padding: 1em 1.4em;
  border-radius: 40px;
  background: rgba(255,255,255,0.15);
  color: #fff
}

.modal-form #keep_signed_in {
  width: auto;
  margin-right: 3px;
}

.modal-form #keep_signed_in + label {
  display: inline-block;
}

하지만 확대를 했을 시 체크박스가 깨지게 되기 때문에 이미지를 넣어서 설정해야 합니다.
체크박스를 ally-hidden 요소로 제거합니다.

.modal-form #keep_signed_in + label::before {
  content: '';
  display: inline-block;
  background: url("../images/icons/icon-no-check.svg") no-repeat;
  background-size: cover;
  width: 12px;
  height: 12px;
  vertical-align: -2.5px;
}

.modal-form #keep_signed_in:checked + label::before {
  background: url("../images/icons/icon-check.svg");
}

.modal-form button[type="submit"] {
  width: 100%;
  margin-top: 15px;
  border: none;
  border-radius: 30px;
  padding: 1em;
  background: $1160ef;
  color: #fff
}

.modal-form button[type="submit"]:hover {
}

select박스에는 css를 넣을 수 없습니다.
그래서 div와 span과 ul과 li요소로 꾸밉니다.

셀렉트 박스 꾸미는 방법
https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_build_custom_form_controls
```


</details>

<details id="1week">
  <summary>첫번째 오프라인 강의</summary>

  
  <br>
  <b>[환경세팅]</b>

  - Web Browser 
  ```
  1. Chrome  - 크롬이란 구글이 개발중인 프리웨어 웹 프라우저다.    
  2. Firefox - 파이어 폭스란 모질라 재단과 모질라 코퍼레이션이 개발한 자유 소프트 웨어 웹프라우저이다.   
  ```

  난 항상 모질라, 파이어 폭스에 대해서 궁금했다. 왜냐하면 쓰지는 않고 듣기만 했기 때문에 하지만 다음과 같은 링크에서 모질라에 대해서 잘 나와있다. 모질라에 대한 내용을 적으면 더러워 보일 수 있어서 다음에 볼 수 있게 링크만 남기도록 하려고 한다.   
  https://firefoxinside.tistory.com/8  
  <br>
  - Web Browser Extension
  ```
  1. Web Developer - 각종 요소들을 비활성화 시키거나 Javascript, CSS, img등을 비활성화시켜 여러 환경을 위한 테스트 가능하다.
  2. HeadingsMap   - HTML5 구조를 파악해주는 도구이다.
  3. OpenWAX       - 웹 접근성 평가 도구이다.
  4. tota11y       - 명도 대비, 문서 아웃라인을 확인해주는 확장 프로그램이다.
  5. Gitzip For Github - 이것을 사용 하기 위해서는 깃허브에서 키를 받아야 한다. 사용법은 해당 확장프로그램 페이지에 잘나와
  있다. 다운로드 하려는 깃허브 파일에 오른쪽 마우스를 클릭하면 해당 아이콘 표시가 떠서 클릭시 다운이 된다.
  ```
  Web Developer 같은 경우에는 해커한테 하이재킹 공격을 당해 광고를 인젝션하여 보여줄 수 있게 해킹했다고 한다. 와 재미겠다..    
  <br>
  - Visual Studio Code
  ```
  1. Visual Studio Code - 말이 필요한가?
  ```

  <br>
  
  - Visual Studio Code Extension
  ```
  1. Korean Language Pack for Visual Studio Code - 모든 text를 한국어로 변환시켜주는 익스텐션이다
  2. Live Server      - VS Code에서 간이 로컬 서버를 시작할 수있는 확장 라이브러리 서버다. 파일업데이트를 자동으로 감지해서 
  매번 리로드를 해주지 않아도 되서 시간을 줄일 수 있다.
  3. Auto Complete Tag - 자동 닫기 태그, 자동 이름 바꾸기 태그 기능이 있다.
  4. Auto Rename Tag   - 짝을 이루는 태그가 수정 될때 같이 수정이 된다.
  5. vscode-icons      - vscode의 아이콘 들을 파일별로 이쁘게 만들어준다. 기존에 쓰던 아이콘 확장이 있다면 설정에서 
  바꾸면 이뻐진다.
  6. Monokai-Contrast Theme - 에디터의 색깔과 코드를 바까준다. 유명한 확장이라 이미 설치가 되어있다. 너무 이뻐서 
  눈이 사라질 것같다.
  ```

  <br>
  <b>[실습파일]</b>  

  우리가 4주동안 만들어야할 실습 파일을 미리 주셨다.  
  https://github.com/seulbinim/exRWD  
      
  위 링크에서 깃 클론 주소를 받아서 내 파일에 추가 할 수 있다.
  VSCODE로 가서 보기 -> 터미널 하게 되면 밑에 터미널 창이 열리는데 처음에는 bash로 되어있지 않아서 powershell부분을 클릭하여 기본셀 선택을 눌러서 bash로 바까주어야 한다. 꼭 해줘야 하는지는 모르겠다.   
  클론 받는 명령어
  ```
  자기가 넣고 싶은 폴더로 cd 명령어를 통해 이동해서 밑 명령어를 치면 된다. 
  git clone 주소
  ```

  여기서 김데레사 강사님꼐서 레파지토리를 파고 그 레파지토리에 넣는 것을 설명 해주셔야 했었는데 너무 짧은 시간에 많은 것을 가르쳐 주실려다보니 레파지토리를 파는 것을 생략하고 넣는 방법만 설명해주셔서 몇분의 수강생이 못따라하고 가만히 앉아있었다. 나는 깃을 써본적이 있어서 그대로 진행을 했다. 이것을 말씀드려야하는지 괜한 참견은 아닌가해서 일단은 가만히 앉아서 내 할일 했다.

  맨 앞에 앉으면 다른 수강생은 잘하는 데 나만 못하는 건가 라는 생각이 들 수 있어서 나는 강의를 들으러 갈때 대부분 맨뒤에 앉아서 수강생분들의 반응을 보는 편이다.

  자기 자신의 레파지토리를 하나 판 뒤에 페이지에 클론 주소가 나오고 그 주소로 파일을 올리면 된다.

  ```
  해당 폴더에 git 파일이 있어서 설정이 되어 있기 때문에 rm -rf 라는 명령어로 git 파일을 삭제한다. rm -rf 
  명령어는 강력하기 때문에 특별한 경우가 아닌 경우 사용하면 안된다고 아는 분에게 들었다. 아는 분이 멍때리다
  가 서버 파일을 다 지운 적이 있어서 rm -rf * 하면 깔끔하게 지워진다.
  - rm -rf .git

  git 파일을 지웠으면 깃 저장소를 만들어 줘야한다.
  - git init

  그리고 복제한 파일을 깃에 올려줘야한다. 아까 복사했던 링크를 적어주면 된다.
  - git remote add origin 주소
  - git add . 
  - git commit -m '설명'
  - git push origin master

  깃 푸시를 할때 이미 계정이 있다면 권한 에러가 뜰텐데 제어판에가서 자격 증명을 해줘야 한다. 계정이 등록이 안되어있다면 
  그대로 로그인 창이 뜨기 때문에 로그인 해주면 된다.
  https://infinitejava.tistory.com/67
  ```

  VSCODE로 들어가 !를 쓰고 엔터를 누르면 HTML을 자동으로 생성해준다.
  ```
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
  </head>
  <body>
    
  </body>
  </html>
  ```

  이러한 코딩 치팅 단어는 에밋이라는 사이트에서 얻을 수 가 있다.
  https://emmet.io/download/  
  너무 신기하다.
  https://code.visualstudio.com/docs/editor/emmet  

  <br>
  <b>[HTML5 탄생]</b><br>
  HTML5는 새로운 표준입니다. 최초버전은 1993년, 최신버전은 1999년에 발표했습니다.   
    
  W3C라는 곳은 웹 표준을 만드는 곳인데. W3C가 XHTML을  1.0을 2.0으로 만들다보니까 호환상에 치명적인 문제가 있어서 개발이 늦어지는 상황이였습니다. 하지만 2004년에 애플, 모질라 재단, 오페라 소프트웨어가 공동으로 만든 WHATWG를 만들고 W3c와 별개로 Web Application 1.0과 Web Forms 2.0을 만들자 아무리 W3C가 표준을 만든다고 하더라도 WHATWG의 프로그램을 많이 쓴다면 표준이 쓸모 없기 때문에 W3C는 위기감을 가지고 2.0의 실패를 인정하고 WHATWG에 합류를 함으로써 W3C와 WHATWG가 공통으로 개발을 하였다. 그리고 HTML5가 된 이유는 시장의 안착을 위해서 HTML5 라고 정하게 되었습니다.  
  <br>
  <b>[콘텐츠 모델]</b>      
  HTML에서는 코딩 규칙에 맞게 하면 안되는 부분이 있다. 하지만 공통적인 부분을 2번 사용하게 되다보니까. 이것을 한번에 쓰기 위해서 콘텐츠 모델이 나왔다. 명확한 정보 구조 설계 및 구성을 위해 카테고리를 정의하여 각 요소별로 비슷한 성격을 가지고 있는 것끼리 그룹화하였는데 이것을 콘텐츠 모델이라고 한다.    
  <br>
  <b>[아웃라인 알고리즘]</b>         
  아웃라인 알고리즘이란 웹 페이지의 정보 구조를 판별 수 있는 개념이다. 예전 같은 경우에는 div를 사용하여 구조화 하였지만 HTML5에서 많은 태그를 지원함 으로서 구조를 판별하기가 쉬워졌다.    
  <br>
  <b>[HTML API]</b>     
  인터넷이 끈어져도 데이터가 남아서 유지를 할 수 있다. 라는 내용으로 설명해주셨다. Web Worker에 대해서 말씀해주셨는데. 이거 설명해주실 때 다른 생각해서 못들었다. 질문 받는 시간에 말하고 싶었는데 내가 설명 못들은 것에 대해 물어보는 건 너무 양심이 없어보여서 패스 했다.    
  <br>
  <b>[CSS]</b>   
  css는 Cascading Style Sheet 마크업 언어이다. 이 부분에 대해서 가능 우선시 할것을 3가지 적어 주셨는데 매우 당연한 애기라서 적지 안았다. 1. 상속 2. ??? 3. 우선순위 였는데 2번째꺼가 기억이 안난다. 술먹고 일어났더니 기억의 절반이 사라진 느낌이다. css 과거의 배치하는 언어는 자유롭지 않았지만 지금 같은 경우 매우 자유로워 졌다고 한다. CSS 같은 경우 버전을 쓰지 않고 레벨을 사용 한다고 한다. 현제 CSS버전은 2.1이 최신 버전이고 CSS3 이라고 들어 봤을텐데 이건 아직 마케팅적인 언어라고 했다. CSS3은 양이 너무 많아서 모듈단위로 개발중이라고 한다.   
  <br>
  <b>[웹표준 개발 단계]</b>   
  웹 표준은 생각보다 많은 과정을 거쳐서 만들어 진다는 것을 알았다. 얼마나 노력했을 까 생각하면 머리가 아프다.
  ```
  초안 - 작업초안 - 권고 후보- 최종 권고안 - 권고안
  ```
  <br>
  <b>[도움이 되는 홈페이지]</b><br>
  그라우스 브라우징

  ```
  css3Test.com
  해당 디바이스가 css를 얼마나 지원 하는지 테스트를 할수있다. 크롬 같은 경우 65%, 마이크로 엣지같은 경우 40% 만약 
  개발할 때 모든 사이트에 돌아갈 수 있도록 개발을 해야한다. 그리고 클라이언트가 어떤 홈페이지 지원을 원하는지 반드시 
  물어봐야한다. 만약 개발시 내가 알아서 할게요 라는 식으로 말하면 클라이언트는 해줘야 되는 입장이여서 모든 페이지에서
   돌아가게끔 만들어야 한다. 만약 클라이언트가 더 많은 지원을 원한다면 비용이 더필요하다라든가 시간을 좀더 달라고 해야
   한다. 만약 그런 것도 안물어 볼시 나중에 소송 싸움이 일어날 수 있다.
  ```

  테스트
  ```
  아까 깔아둔 web Developer를 사용하여 Tools -> Validate Local Html을 들어가서 확인 할 수 있다.
  ```

  css 실무 코딩을 볼 수 있는 사이트
  ```
  http://www.csszengarden.com/214/page2/ 사이트를 들어가면 같은 페이지이지만 여러 CSS 적용 
  시켜서 다른 디자인의 홈페이지를 만든 것을 확인할 수 있다. VIEW ALL DESIGNS는 주소 오류가 있는지 
  바로 밑에 있는 글을 누르면 다른 사람이 한 것을 볼 수 있다.
  ```

  <br>
  <b>[구글 SEO]</b><br>
  검색엔진 최적화를 SEO라고 한다. SEO를 사용 하지 않고 그대로 웹개발을 하게 되면 해당 홈페이지에 대한 홍보는 누가 할 것인가? 아무리 잘만든 홈페이지라도 수익을 내고 싶다면 수익의 절반은 마케팅 비용으로 사양해야 한다. https://www.twinword.co.kr/blog/search-engine-optimization-guide/    
  <br><br>
  <b>[!important의 쓰임새]</b><br>

  ```
  해당 important라는 것은 우선순위를 최고로 만들어 준다. 사용하는 경우는 2가지이다.
  1. 동적인 스타일 (팝업창 같은? 먼가 티어나오는 것을 말하는 것같다. 이것을 질문을 안하다니..)
  2. 테스트 용도 
  ```

  이번 프로젝트에서 부트스트랩 달력을 커스텀 할때 우선순위에 대해서 알고 있었지만 너무 귀찬아서 important를 사용했다. 만약 사용하게 된다면 그것을 덮어쓰기위해 계속적으로 css를 만들어 줘야한다. 그만큼 코드량이 들어나고 더럽게 짜증나고 오래걸린다. 아무리 무슨일이 있어도 important를 사용하지 말고 우선순위 규칙을 사용하여 작성해야한다. 이것때문에 4일동안 달력만 만졌다.

  <br>
  <b>[나중에 검색하려고 필기한 것들]</b><br>

  ```
  figma
  3단구조 4단구조 (네비게이션을 헤더에 분리하거나 포함할 수 있다.)
  기계 처리도 가능한 것. 시멘틱 마크업
  ARIA
  ```

  <br>
  <b>[많은 표기 방법]</b><br>
  똑같은 기능을 하는 HEADER나 FOOTER같은 경우 혼동이 올 수 있기떄문에 ID나 CLASS를 사용해서 표기를 하는데, CLASS를 많이 사용하기때문에 CLASS를 사용 하는 것이 좋다.

  - 표기방법 

  ```
  1. pc 파스칼 케이스    MainContain   - 단어의 앞에를 대문자로 사용
  2. CC 카멜 케이스      main-contain  - 낙타처럼 생겼다고 해서 카멜이라고 한다.
  3. KC 케밥케이스       main-contain  - 음?? - 사용해서 끈으면 된다.
  4. SC 스네이크 케이스  main_contain  - 뱀처럼 밑에 달아서 스테이크 케이스라고 한다.

  BAM 방법론
  https://webclub.tistory.com/263

  네이밍 규칙
  http://darum.daum.net/convention/name
  ```

  파스칼과 카멜 같은 경우에는 백엔드인 나에게 많이 쓰인다. 가끔 코딩하다가 BAM방법론 코드를 본적이 있는데, 저사람은 왜 오타를 냈지 라고 생각을 했었다. 근데 저게 요즘 많이 쓴다고 하니까 꼭 봐야할것같다.

  <br>
  <b>[전역속성]</b>   

  ```
  모든 요소에 적을 수 있는 속성들을 전역 속성이라고 한다.
  이 태그가 어떤거냐고 물어보셨는데 내가 중간에 놓친게 있는 것 같다.
  title, lang, id, class, style, data-* 등이 있다.
  data-* 같은 경우 난 많이 사용해서 알지만 모르는 사람이 꽤나 있다.
  ```

  Lang = 'KO-KR' KO는 한국어이고 KR 같은 경우는 한국을 나타낸다. 한국어을 사용하는 나라가 2개 있어서 코리안 리퍼블릭이라는 표시다.

  <br>
  <b>[실습HTML]</b>   

  ```HTML
  네이버 로그인 폼을 보면서 개발을 할시에 따로따로 만드는 것이 아니라 위에서 아래로 한다음에 부가적인 것을 추가한다고 했다.

  !를 쓰고 엔터를 써서 기본적인 태그르 생성한다.
  div.container를 쓰고 엔터를 누르면 div에 container 클래스를 가진 요소가 생성된다.

  div.container 
  <div class="container"></div>
  div#container
  <div id="container"></div>

  +를 사용하게 되면 자식 요소를 만들 수 있다. 이 부분에서 엄청 신기했는데 너무 조용해서 속으로만 신기해 했다.
  header.appHeader+mav.appNavigation+main.appMain+footer.appFooter

  <header class="appHeader"></header>
  <mav class="appNavigation"></mav>
  <main class="appMain"></main>
  <footer class="appFooter"></footer>

  다음과 같이 작성한다.

  <!DOCTYPE html>
  <html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
  </head>

  <body>
    <div class="container">
      <header class="appHeader">헤더</header>
      <mav class="appNavigation">네비게이션</mav>
      <main class="appMain">
        <section class="book">추천서적</section>
        <section class="news">새소식</section>
        <section class="board">게시판</section>
        <section class="favorite">인기사이트</section>
        <article class="twitter">트위터</article>
      </main>
      <footer class="appFooter">푸터</footer>
    </div>
  </body>

  </html>

  이렇게 한다음에 web developer를 사용해서 outline에 outline Block Level Elements를 사용해서 블록을 표시해준다.
  컨테이너가 감싸는 것을 볼 수 있다.

  section[class]
  section[class]*4
  section.main$*4
  section.main$*4{메인$}

  *4 => *숫자 하면 숫자 개수 만큼 요소가 만들어진다 
  $  => 달러 표시를 사용 할시 index값이 나온다.


  section.main$*4{메인$}
  <section class="main1">메인1</section>
  <section class="main2">메인2</section>
  <section class="main3">메인3</section>
  <section class="main4">메인4</section>

  해당 치팅에 대해서 더 보고 싶다면 에밋 사이트를 참고하면 된다라고 말씀 하셨다.

  tools Validate Local Html 사용해 웹 접근성을 확인해보면 mav 부분이 오타가 나고 섹션이랑 이티클 같은 경우 
  H제목을 명시적으로 써줘야 한다고 한다. H제목을 써주는 거에 대해서는 다시 한번 인강을 찾아서 볼 생각이다. 잘 생각이 안나서.

  mav를 nav로 고쳐준다.

  기본적인 구조를 만들었으니 

  헤더에 css파일을 명시해준다.
  <link rel="stylesheet" href="./css/main.css">

  HTML 완성본
  <!DOCTYPE html>
  <html lang="ko-KR">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>웹카페-HTML5, CSS3</title>
    <link rel="stylesheet" href="./css/main.css">
  </head>

  <body>
    <div class="container">
      <header class="appHeader">헤더</header>
      <nav class="appNavigation">네비게이션</nav>
      <main class="appMain">
        <section class="book">추천서적</section>
        <section class="news">새소식</section>
        <section class="board">게시판</section>
        <section class="favorite">인기사이트</section>
        <article class="twitter">트위터</article>
      </main>
      <footer class="appFooter">푸터</footer>
    </div>

  </body>

  </html>
  ```

  <br>
  <b>[실습CSS]</b>  

  ```
  컨테이너는 기본적으로 margin 값을 가지고 있어서 0으로 해줘야합니다.

  그리고 폰트 기본적은 폰트사이즈를 HTML css 를 넣어주고 하게되면 관리하기가 더 편합니다.


  m0 -> margin 0
  fsz -> font0size

  html {
    font-size: 10px;
  }

  body {
    margin: 0;
    font-size: 1.4em;
  }

  그리고 구조화를 눈으로 확인 할 수 있도록 색깔을 넣어줍니다.
  body {
    background-color: yellow;
  }

  .container, .appMain {
    background-color: silver;
  }

  .appHeader {
    background-color: pink;
  }

  .appNavigation {
    background-color: lime;
  }

  .appMain {
    background-color: blue;
  }

  .book, .news, .board, .favorite, .twitter {
    background-color: skyblue;
  }

  .appFooter {
    background-color: orange;
  }

  모바일 같은 경우는 구조가 싶지만 데스크탑인 경우 요소가 많습니다라고 설명해주셨고
  개발할떄는 모바일 먼저 개발하고 데스크탑을 이후에 개발하신다고 하셨다.

  컨테이너를 이제 플렉스로 만들어줍니다.
  display: flex;

  그리고 flex-flow를 colume으로 바까줍니다.

  미디어 쿼리를 가서 vh를 사용해서 길이를 설정해줍니다.

  /* 모바일 디바이스 */
  @media screen and (max-width: 999px){
    .appHeader, .appMain {
      width: 100%;
    }

    /* 모바일 헤더 */
    .appHeader {
      height: 10vh;
    }

    /* 모바일 네비게이션 콘텐츠 */
    .appNavigation {
      height: 20vh;
    }

    /* 모바일 메인 콘텐츠 */
    .appMain {
      height: 50vh;
    }

    /* 모바일 푸터 */
    .appFooter {
      height: 20vh;
    }
  }

  창을 999px로 줄이게 되면 전부다 한줄이 된다. 근데 여기서 먼가 중요한 애기를 해줬을 거 같은데 다른 곳에 집중이 되서 
  이 부분을 못들은 게 너무 아쉽다...  
    
  그러면 모든 요소가 가로로 배치되는 데 순서를 바꾸고 싶다면 order라는 속성을 이용해서 0과 1을 등을 사용해서 바꾸면 됩니다. 
  만약 맨위로 올리고 싶을때 -1을 사용 하면 됩니다.

  그리고 다시 flex-flow를 row로 바까줍니다.

  그리고 모든 값을 100%로 만들어줍니다.

  셀럭터 그룹핑을 통해 작성
  .book, .news, .board, .favorite, .twitter {
      width: 100%;
      height: 10vh;
  }

  appMain이 50vh이기 때문에 10vh씩 할당 된 것을 볼 수 있다.

  여기서 적지말고 보기만 하라고 하셨다.
  flex-direction을 row로 주고 width값을 수정하게 되면 화면이 이상하게 나온다.
  그래서 flex-wrap을 사용해서 줄바꿈을 허용 해줘야한다.

  flex-direction: row;
  flex-wrap: wrap;

  위에 값을 동시에 적어주면 편하다. 요즘은 밑에 코드처럼 많이 작성합니다 라고 말씀하셨다.
  flex-flow: row wrap;

  그 다음은 데탑을 쭉 설정 해줬다.
  일단 내 코드에 에러가 있어서 해결 후 작성 하려고 한다.

  왜 코드가 이상한지 했더니 모바일 미디어 쿼리 max-width를 999px이 아닌 900으로 설정해서 이상한 거였다.
  다음에는 더 집중해야겠다.

  그 다음에는 밑에 있는 요소에 대해서 설명해 주셨다. 설명이 기억이 안나서 인터넷에서 검색한 내용으로
  정의하겠습니다. Flex 요소에서 사용가능
  justify-content : 가로축 - 중심축
  align-items     : 세로축 - 교차축
  https://ipex.tistory.com/entry/CSS3-flex-Box-justifycontent-alignitems

  /* 데스크탑 디바이스 */
 @media screen and (min-width: 1000px){

 }
 
 모바일 데스크탑의 길이가 최소 1000px일때 
 헤더는 가운데와 appMain은 1000px로 설정해주고 
 container 같은 경우 가운데 정렬을 해야 되기 때문에 

 justify-content: center; 설정해야한다.

 그리고 appMain안에 있는 컨텐츠들은 동일한 간격을 가져야 함으로 
 justify-content: space-between; 사용해서 동일한 간격을 가지게 만든다.

 여기서부터 길이를 계산해서 칠판에 써주셨다.
 생각해보니까 그 적어주신거 카메라로 찍어야지 생각하고 있다가 깜박하고 안찍었는데 혹시라도 찍은 사람이 있을까.. 없겠지 젠장

 /* 데스크탑 디바이스 */
@media screen and (min-width: 1000px){
  .appHeader, .appMain{
    width: 1000px;
  }
  /* 데스크탑 컨테이너 */
  .container{
    justify-content: center;
  }
   /* 데스크탑 헤더 */
   .appHeader{
    height: 10vh;
  }
  /* 데스크탑 내비게이션 */
  .appNavigation{
    height: 20vh;
  }
  /* 데스크탑 메인 콘텐츠 */
  .appMain{
    height: 60vh;
    justify-content: space-between;
  }
  /* 데스크탑 추천 서적 */
  .book{
    width: 320px;
  }
  /* 데스크탑 새소식 */
  .news{
    width: 660px;
  }
  /* 데스트탑 게시판 */
  .board{
    width: 320px;
  }
  /* 데스크탑 인기 사이트 */
  .favorite{
    width: 240px;
  }
  /* 데스크탑 트위터 */
  .twitter{
    width: 400px;
  }
  /* 데스크탑 푸터 */
  .appFooter{
    height: 10vh;
  }
}

마무리하고 교육이 종료가 되었다.
해당 정리 내용은 1달 교육기간이 지나면 비공개로 만들고 pptx로 정리하여 소장할 생각이다.
오늘은 쫌 일찍들어가서 내일 아침에 일찍 회사로 와서 리액트를 공부할 예정이다.
  ```


</details>

<details id="1weekReview">
  <summary>첫번째 오프라인 강의 후기</summary>

  <b>[새벽인데. 오후에 안하고 왜 새벽에 작성하는지에 대한 이유]</b>  
  금일 친구가 저녁에 약속이 있다고 해서 오후 술을 먹고 고시텔을 가서 뻗어 버렸습니다. 잊기 전에 빨리 배웠던 내용을 작성하려고 합니다. 새벽이라 그런지 감수성이 풍부해 질것같습니다.  

  <b>[수업 전 후기]</b>    
  처음에 일찍 와서 강사님이랑 야무님과 이야기를 할 수 있었다. 야무님 강의 같은 경우 페스트 캠퍼스에서 강의를 시청한 적이 있어서 페스트 캠퍼스 강의를 볼 때 완강을 했지만 별로 남지 않았다. 그래서 오프라인 모이기 전에 각 잡고 공부하려고 했는데 그렇게 쉽진 않았다. 이번에 50만 원이라는 강의를 살면서 처음 질러 봤다. 그리고 생각보다 야무님처럼 잘하고 싶다는 로망이 있었는지 왜 나이가 많을 거라고 생각했을까.  
    
  회사에서 전부 지원해 주신다고 했는데 내 돈으로 듣지 않는 수업이라면 무슨 의미가 있겠는가 싶다. 대놓고 거절하면 회사에서 이녀석 나갈려고 설계하는건가 라고 생각 할 수 있으니까. 정중히 설명 드리는 게 좋다. 제 돈으로 하고 싶다고 했는데. 착하신 이사님께서 절반을 지원해준다고 하셨다. 그래서 회사에서 절반을 지원받고 새벽에도 공부하며 열심히 하고 있다.   

  강의는 1~2시간이지만 정리를 해서 내 것으로 만드는 시간이 3시간 정도 걸린다. 처음 오신 분이 열심히 하는 분이 2명 있다고 말씀하셔서 나는 아니겠지 생각했는데. 깃허브에 이런 식으로 숙제를 하라고 하셔서 '음 그렇게 하는 거구나' 생각했는데, 뭔가 잘못되었다는 걸 느꼈다. 어차피 시작한 거 그냥 해야겠다. 이것도 나름 재미있어서 이렇게 취향이 공개되는 건가. 머리카락이 빠져서 스티브 잡스님처럼 될것같지만 성취감이 너무 좋다. 혜진님께서는 열정이 대단하신거 같은데. 저렇게 열정적인 분들이 나중에 회사 주요 인력이 되거나 실력파가 될 가능성이 크다. 회사에서 적극적으로 지원을 해준다면 실력이 금방 커질 수 있을 것 같다.   

  나같은 경우에는 게임 중독자에서 개발자가 되서 한가지에 집중하게 되면 시간이 가는 줄 모르고 밤새는 거에 익숙하다. 백수에서 개발자로 이직을 잘한 케이스가 아닐까?. 게임을 너무 많이해서 밤새서 게임을 하는 것보다는 점심시간에 게임을 하고 밤에는 공부를 한다. 우리회사는 엄청 프리한 편이라 개발 일정만 마추면 머든지 해도 된다고 했다.    
    
  <b>[수업후 후기]</b>  
  오늘 너무 보람찬 시간을 보냈던거 같다. 가격이 싸거나 국비 과정 같은 경우에는 교과서 읽는거 마냥 수업을 들었었는데. 비싼 강의를 들어보면 말 하나하나가 명언 같다. 내가 알고 싶은 내용도 있고 처음 듣는 내용 너무 재미 있었다. 가서 진짜 궁금했던 것을 직접 물어보고 내 공부에 대해서 확답을 들을 수 있었다.   
     
  '6월달에 회사에서 리액트 프로젝트를 진행하는데 리액트를 공부하는 데 얼마나 걸릴거 같으세요' 라는 질문을 했었는데 야무님께서 '그건 사람마다 다르잔아요' 라고 말씀하셨다. 이말을 듣고나니 책의 앞장만 보고 시간이 없다는 핑계(?)만으로 공부를 시작도 안했다. 답은 간단 했던거 같다. 잠자는 시간을 줄여서 리액트를 공부할 수 있는 시간까지 만들면 되는 것이 아닌가 라는 생각이 들었다.  

  그리고 회사에서 디자이너가 이미지를 주고 해당 이미지처럼 개발해달라고 했는데. 눈 대충으로 코딩을 하니까 옆 디자이너가 '왜 그렇게 코딩하세요?' 라고 화를 내는 거보고 나는 이게 프론트 엔드가 이미지를 일일이 계산해서 하는 건줄 알았다. 그래서 아침에 야무님이랑 김데레사 강사님에게 어떻게 구하는 지 말씀드렸을때 왜 이해를 못하시나 했었는데 이게 디자이너가 협업 도구를 통해 줘야 한다고 했다. 친절하게 설명해주신 야무님에게 감사하고 디자이너에게 약간 억울하고 실망감이 들었다.

  김데레사 강사님 강의는 9시부터 13시 까지 진행 되었고 열심히 설명해주셔서 짧은 시간이였지만 많은 설명을 들을 수 있었다. 열심히 설명을 듣다가 질문을 하셨는데 너무 설명을 열심히 들어서 질문 하셨는지도 몰랐다. 열심히 듣고 있었는 데 1000 / 140이 머였냐는 질문이 나와서 순간 뇌 정지가 왔었다. 플렉스에 대한 질문도 하셨는 데, 이건 다음주부터 듣는 온라인 강의였다고 혜진님이 말씀하기 전까지는 나는 내가 온라인 강의에서 빠트린게 있었나 싶었다.

  오늘 열심히 강의 해주신 김데레사 강사님에게 감사하고 친절하게 질문에 답해주신 야무님에게 또 한번 감사합니다. 이번주도 더 열심히 살아야겠습니다.
</details>
