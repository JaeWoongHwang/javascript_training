### Web Design

#### Flat Design

Why? 모바일 디바이스에 최적화된 디자인이기 때문.

How? 

- 직관적이고 단순하게 만들어라.

- 색상은 6~8가지의 최소화된 색상만을 사용해라. 단순한 도형을 사용하는 대신 밝고 화려한 색상을 선택한다.

  ~~~ R
  플랫 디자인 시 색상 선택에 도움을 줄 사이트
  flatuicolors.com
  ~~~

- 간결하면서 인상적인 타이포그래피

  - 인상적인 문구를 강조해서 보여준다.
  -  화려한 특수 글꼴을 많이 사용하거나 글자에 효과를 많이 넣으면 직관성에 방해 될 수 있다.



#### Material Design

웹과 앱을 통틀어 모든 개발 플랫폼에서 사용자 경험을 하나로 묶기 위해 구글이 제시한 디자인 방법.

~~~
구글 '머터리얼 디자인 어워드'
design.google/library/material-design-awards-2017
2017년 수상 디자인 확인 가능
~~~

머터리얼 디자인 라이트 프레임워크 활용하기 

~~~
getmdl.io 참고
~~~



#### Card Design

카드형 디자인 장점

- 콘텐츠 중심의 박스 형태로 시선 사로잡기
  - 박스로 콘텐츠가 분리되어 있기 때문에 텍스트가 죽 나열되어 있는 사이트보다 훨씬 많은 양의 정보를 한눈에 파악하기 쉬움
- 레이아웃을 자유자재로 바꿀 수 있음
- 지나친 스크롤을 줄일 수 있음



카드형 디자인 단점

- 레아아웃에 큰 변화를 줄 수 없음
  - 사용자에게 계속 비슷한 UI를 제공하는 한계
- 카드 안에 담아야 할 내용이 많거나 콘텐츠를 비교해가며 훑어봐야 할 사이트에는 적합하지 않음



#### Grid System

What? 페이지나 화면에 정보를 구성할 때 논리적으로 일관성 있게 표현하기 위한 구조

Why? 화면을 규칙적으로 배열하기 때문에 레이아웃을 일관성 있게 유지할 수 있음.

~~~
크롬의 'Design Grid Overlay'확장 프로그램을 사용하면 웹 사이트의 그리드 시스템을 눈으로 확인할 수 있음.
~~~

그리드 시스템은 화면 너비를 몇 픽셀로 하는가에 따라 구분하기도 하고, 한 화면에 칼럼이 몇 개인가를 기준으로 구분하기도 한다.

그리드 레이아웃의 특징

- 시각적으로 안정적인 디자인
- 단순한 웹 디자인
- 내용을 원하는 대로 배치



#### Typography

**웹 화면 배경 색상과 타이포그래피 색상의 대비**

웹 디자인에서 놓치지 말아야 할 부분은 사이트 배경과 어울리도록 텍스트 색상을 선택하는 것이다.
색상 대비 체크 시뮬레이트 사이트

~~~
https://webaim.org/resources/contrastchecker/
~~~

위 사이트를 통해 웹 콘텐츠 접근성 지침(WCAG)에 적합한지를 판단할 수 있다. 웹 콘텐츠 접근성이란 장애인도 웹 사이트를 불편함 없이 사용할 수 있도록 설계하는 것이다.



#### Media Query

미디어 쿼리를 사용하기 위해서는 CSS를 정의하는 <style>태그 안에 다음과 같은 구문을 삽힙한다.
이때 대소문자는 구별하지 않는다.

~~~
기본형식
@media [only|not]미디어 유형 [and조건]*[and조건]
~~~

- @media : 스타일 시트 안에서 미디어 쿼리를 시작하는 속성
- only | not : 미디어 쿼리를 적용할 유형을 지정할 때 사용하는 접두어. only 접두어를 사용하면 only 다음의 미디어 유형에만 적용되고, not을 사용하면 not 다음의 미디어 유형을 제외한 나머지 유형에만 적용된다.
- 미디어 유형 : 화면인지 프린터인지, TV인지 등 미디어 쿼리를 적용할 기기를 지정하는 부분. 쉽표를 사용해 여러가지 미디어 유형을 나열할 수 있다.
- 조건 : 미디어 유형 외에 기기와 관련된 조건을 지정한 후 해당 조건에 맞는 경우에만 CSS를 적용하도록 지정할 수 있다. 조건은 괄호로 묶어서 표현하며 둘 이상의 조건을 나열할 경우 and 연산자를 사용한다.



**미디어 쿼리 중단점**

미디어 쿼리를 작성할 때 화면 크기에 따라 서로 다른 CSS를 적용할 분기점을 중단점(Break Point)라고 한다. 
**과거에는 모바일, 태블릿, 데스크톱처럼 기기 중심으로 미디어 쿼리 중단점을 나누었지만 다양한 업체에서 새로운 기기가 계속 등장하고 바뀌는 속도도 빠르기 때문에 기기를 기준으로 하는 것은 바람직 하지 않다.**

중단점을 정할 때는 콘텐츠를 기준으로 하는 것이 좋다. 우선 작은 화면을 기준으로 콘텐츠를 제작하고 화면을 점점 늘려나가다 콘텐츠 배치를 다르게 해야 할 크기가 되면 중단점을 추가한다.

시중의 모든 디바이스를 반영할 수 없기 때문에, 주로 작은 화면과 중간화면, 큰화면 정도로 구분 짓고 필요할 경우 좀 더 세분화 하기도 한디. 그리고 처리 속도나 화면 크기 등에서 다른 기기보다 모바일 기기의 제약 조건이 더 많기 떄문에 모바일 기기의 레이아웃을 기본으로 하여 CSS를 만든다. 그리고 나서 좀 더 사양이 좋고 화면이 큰 태블릿과 데스크톱에 맞춰 더 많은 기능과 스타일을 추가하는데 이렇게 모바일을 먼저 고려하여 미디어 쿼리를 작성하는 것을 '모바일 퍼스트'라고 한다.

~~~
기기별로 자세한 중단점을 알 수 있는 사이트
css-tricks.com/snippets/css/media-queries-for-standard-devices
~~~



**미디어 쿼리를 지원하지 않는 브라우저에 대응하려면**

국내 사용자가 많은 인터넷 익스플로러 브라우저의 6~8버전에서는 반응형 웹이 동작하지 않는다. 인터넷 익스플로러 6~8버전을 비롯해 미디어 쿼리를 지원하지 않는 브라우저에서도 반응형 뒙이 동작하도록 설계하려면 respond.js 자바스크립트 라이브러리를 다운로드해서 링크하면 된다.

respond.js를 다운로드 하려면 

~~~
github.com/scottjehl/Respond 페이지로 들어가 git clone - Download Zip을 한다.
파일의 압축을 푼 후 src/respond.js 파일을 원하는 폴더로 복사한다.
~~~

그리고 CSS의 조건 주석문을 사용해 인터넷 익스플로러 9 이하 버전일 경우 respond.js파일을 가져오는 소스를 작성한다. respond.js 파일 경로를 표시할 떄는 폴더 이름까지 함께 표기해야 하는데, 만일 script 폴더 안에 저장했다면 다음과 같이 작성한다.

~~~
<!--[if It IE 9]
	<script src = "script/respond.js"></script>
<[endif]-->
~~~



**미디어 쿼리 사용하기**

- 외부 CSS 파일로 정의하기

  - link 태그 사용하기

    ~~~
    <link rel="stylesheet" media="미디어 쿼리 조건" href="css파일 경로">
    위의 구문은 특정 조건에 맞는다면 지정한 CSS 파일을 가져와 적용하라는 뜻
    속성 순서는 상관없다.
    
    대표적인 미디어 쿼리 사이트 colly.com의 소스를 열어보면 head태그 안에 link태그를 사용해 화면용 스타일시트 파일 /css/screen.css를 링크한 부분을 볼 수 있다.
    <link href="/css/screen.css" type="text/css" rel="stylesheet" media="screen">
    
    예를 들어 화면 너비가 768px이하일 때 적용할 태블릿용 스타일 시트 파일을 불러온다면
    <link rel="stylesheet" media="screen and(max-width:768px)" hef="css/tablet.css">
    ~~~

  - @import구문 사용하기

    ~~~
    @import url(css파일 경로) 미디어 쿼리 조건
    
    예를 들어 태블릿 PC에 맞는 스타일시트 tablet.css를 만들어 두었고 너비가 321px이상이고 768px이하일 때 적용하고 싶다면 다음과 같이 지정한다.
    
    @import url("css/tablet.css") screen and (min-width:321px) and (max-width:798px);
    ~~~

- 웹 문서에서 직접 정의하기