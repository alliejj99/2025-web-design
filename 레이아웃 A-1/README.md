# 웹디자인개발기능사 레이아웃 A-1

웹디자인개발기능사 시험에서는 총 6가지 유형의 레이아웃이 제시되며, 각 유형마다 4가지 형태가 포함되어 있습니다. 실제로는 유사한 구성들이 많아 유형별로 1~2개씩만 연습해도 충분하지만, 처음 코딩을 접하는 분이라면 반복적인 학습이 중요합니다. 따라서 24개 전체 유형을 모두 따라해보는 것을 추천드립니다. 처음에는 어렵게 느껴질 수 있지만, 꾸준히 따라하다 보면 시험장에서 스스로 코딩을 완성하고 있는 자신을 발견하게 될 것입니다.


## 1. 기본 구조 만들기

`VS Code`를 실행하고 `webdesign` 폴더를 생성 후 `layoutA-1.html` 파일을 만듭니다.  
`!` 입력 후 `Tab` 키를 누르면 기본 HTML 구조가 생성됩니다.  
`lang` 속성은 `ko`, `title`은 `웹디자인개발기능사 레이아웃 A-1`로 변경합니다.

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>웹디자인개발기능사 레이아웃 A-1</title>
</head>
<body>
    
</body>
</html>
전체 구조
이 레이아웃은 header, slider, contents, footer 4개 영역으로 구성되며,
이를 감싸는 wrap 컨테이너를 사용합니다.

html
코드 복사
<body>
    <div id="wrap">
        <div id="header"></div>
        <div id="slider"></div>
        <div id="contents"></div>
        <div id="footer"></div>
    </div>
</body>
초기 CSS 설정
css
코드 복사
* {
    margin: 0;
    padding: 0;
}
#wrap {
    width: 1200px;
    margin: 0 auto;
}
#header {
    width: 100%;
    height: 100px;
    background-color: #efefef;
}
#slider {
    width: 100%;
    height: 300px;
    background-color: #e3e3e3;
}
#contents {
    width: 100%;
    height: 200px;
    background-color: #d9d9d9;
}
#footer {
    width: 100%;
    height: 100px;
    background-color: #d1d1d1;
}
margin: 0 auto; → 블록요소를 가운데 정렬
background-color → 영역 시각화용 임시 색상

2. 각 섹션 작업하기
Header 영역
로고(.logo)와 네비게이션(.nav)으로 구성.
display: flex를 적용하여 가로 정렬합니다.

html
코드 복사
<div id="header">
    <div class="logo"></div>
    <div class="nav"></div>
</div>
<!-- //header -->
css
코드 복사
#header {
    width: 100%;
    display: flex;
}
#header .logo {
    width: 20%;
    height: 100px;
    background-color: #efefef;
}
#header .nav {
    width: 80%;
    height: 100px;
    background-color: #e3e3e3;
}
Slider 영역
html
코드 복사
<div id="slider"></div>
<!-- //slider -->
css
코드 복사
#slider {
    width: 100%;
    height: 300px;
    background-color: #d9d9d9;
}
Contents 영역
3개의 컨텐츠 박스로 구성 (.content1, .content2, .content3).

html
코드 복사
<div id="contents">
    <div class="content1"></div>
    <div class="content2"></div>
    <div class="content3"></div>
</div>
<!-- //contents -->
css
코드 복사
#contents {
    width: 100%;
    display: flex;
}
#contents .content1 {
    width: 33.3333%;
    height: 200px;
    background-color: #d1d1d1;
}
#contents .content2 {
    width: 33.3333%;
    height: 200px;
    background-color: #c7c7c7;
}
#contents .content3 {
    width: 33.3333%;
    height: 200px;
    background-color: #bcbcbc;
}
Footer 영역
3개의 하위 영역으로 구성 (.footer1, .footer2, .footer3).

html
코드 복사
<div id="footer">
    <div class="footer1"></div>
    <div class="footer2"></div>
    <div class="footer3"></div>
</div>
<!-- //footer -->
css
코드 복사
#footer {
    width: 100%;
    display: flex;
}
#footer .footer1 {
    width: 20%;
    height: 100px;
    background-color: #b1b1b1;
}
#footer .footer2 {
    width: 60%;
    height: 100px;
    background-color: #a3a3a3;
}
#footer .footer3 {
    width: 20%;
    height: 100px;
    background-color: #9d9d9d;
}
3. 정리
✅ 주요 HTML 태그
<div> : 기본 블록 요소. 영역 구분용으로 사용.

✅ 주요 CSS 속성
display: flex → 자식 요소를 가로로 정렬

margin: 0 auto → 중앙 정렬

width, height → 박스 크기 지정

background-color → 구조 확인용 배경색

✅ 구조 설계 포인트
#wrap : 전체 레이아웃 컨테이너

#header, #slider, #contents, #footer : 시각적 구분용 영역

내부 섹션은 flex로 정렬

✅ 핵심 요약
기본 HTML + CSS 레이아웃 구조 설계

flex를 활용한 최신 CSS 배치 방식 실습

시험 실무에서는 float 대신 flex 사용 권장

코드 복사






나의 말:
README.md 통으로 주세용



ChatGPT의 말:
markdown
코드 복사
# 웹디자인개발기능사 레이아웃 A-1

## 1. 기본 구조 만들기

`VS Code`를 실행하고 `webdesign` 폴더를 생성 후 `layoutA-1.html` 파일을 만듭니다.  
`!` 입력 후 `Tab` 키를 누르면 기본 HTML 구조가 생성됩니다.  
`lang` 속성은 `ko`, `title`은 `웹디자인개발기능사 레이아웃 A-1`로 변경합니다.

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>웹디자인개발기능사 레이아웃 A-1</title>
</head>
<body>
    
</body>
</html>
전체 구조
이 레이아웃은 header, slider, contents, footer 4개 영역으로 구성되며,
이를 감싸는 wrap 컨테이너를 사용합니다.

html
코드 복사
<body>
    <div id="wrap">
        <div id="header"></div>
        <div id="slider"></div>
        <div id="contents"></div>
        <div id="footer"></div>
    </div>
</body>
초기 CSS 설정
css
코드 복사
* {
    margin: 0;
    padding: 0;
}
#wrap {
    width: 1200px;
    margin: 0 auto;
}
#header {
    width: 100%;
    height: 100px;
    background-color: #efefef;
}
#slider {
    width: 100%;
    height: 300px;
    background-color: #e3e3e3;
}
#contents {
    width: 100%;
    height: 200px;
    background-color: #d9d9d9;
}
#footer {
    width: 100%;
    height: 100px;
    background-color: #d1d1d1;
}
margin: 0 auto; → 블록요소를 가운데 정렬
background-color → 영역 시각화용 임시 색상

2. 각 섹션 작업하기
Header 영역
로고(.logo)와 네비게이션(.nav)으로 구성.
display: flex를 적용하여 가로 정렬합니다.

html
코드 복사
<div id="header">
    <div class="logo"></div>
    <div class="nav"></div>
</div>
<!-- //header -->
css
코드 복사
#header {
    width: 100%;
    display: flex;
}
#header .logo {
    width: 20%;
    height: 100px;
    background-color: #efefef;
}
#header .nav {
    width: 80%;
    height: 100px;
    background-color: #e3e3e3;
}
Slider 영역
html
코드 복사
<div id="slider"></div>
<!-- //slider -->
css
코드 복사
#slider {
    width: 100%;
    height: 300px;
    background-color: #d9d9d9;
}
Contents 영역
3개의 컨텐츠 박스로 구성 (.content1, .content2, .content3).

html
코드 복사
<div id="contents">
    <div class="content1"></div>
    <div class="content2"></div>
    <div class="content3"></div>
</div>
<!-- //contents -->
css
코드 복사
#contents {
    width: 100%;
    display: flex;
}
#contents .content1 {
    width: 33.3333%;
    height: 200px;
    background-color: #d1d1d1;
}
#contents .content2 {
    width: 33.3333%;
    height: 200px;
    background-color: #c7c7c7;
}
#contents .content3 {
    width: 33.3333%;
    height: 200px;
    background-color: #bcbcbc;
}
Footer 영역
3개의 하위 영역으로 구성 (.footer1, .footer2, .footer3).

html
코드 복사
<div id="footer">
    <div class="footer1"></div>
    <div class="footer2"></div>
    <div class="footer3"></div>
</div>
<!-- //footer -->
css
코드 복사
#footer {
    width: 100%;
    display: flex;
}
#footer .footer1 {
    width: 20%;
    height: 100px;
    background-color: #b1b1b1;
}
#footer .footer2 {
    width: 60%;
    height: 100px;
    background-color: #a3a3a3;
}
#footer .footer3 {
    width: 20%;
    height: 100px;
    background-color: #9d9d9d;
}
3. 정리
✅ 주요 HTML 태그
<div> : 기본 블록 요소. 영역 구분용으로 사용.

✅ 주요 CSS 속성
display: flex → 자식 요소를 가로로 정렬

margin: 0 auto → 중앙 정렬

width, height → 박스 크기 지정

background-color → 구조 확인용 배경색

✅ 구조 설계 포인트
#wrap : 전체 레이아웃 컨테이너

#header, #slider, #contents, #footer : 시각적 구분용 영역

내부 섹션은 flex로 정렬

✅ 핵심 요약
기본 HTML + CSS 레이아웃 구조 설계

flex를 활용한 최신 CSS 배치 방식 실습

시험 실무에서는 float 대신 flex 사용 권장