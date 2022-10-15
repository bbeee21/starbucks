# reset cdn
- html 파일 초기화 (브라우저별로 다른 스타일 적용되어 있기 때문)
- 링크 : https://www.jsdelivr.com/package/npm/reset-css

# google material icons
- develop -> web -> getting started
- 2번째꺼
- 링크 : https://material.io/design/iconography/system-icons.html

# google fonts
- 나눔 고딕 사용
- css 불러오기 전에 해당 폰트를 불러오기
- font 기본 사이즈는 16px
- 링크 : https://fonts.google.com/specimen/Nanum+Gothic?query=nanum

## tag
- img태그 : inline 요소 , 높이값을 지정해주고 block 요소로 변환
- 글자 위주의 특성인 inline은 , baseline이라고 하는 글자의 밑에를 담당하는 부분이 존재
- xyzkj 에서 y와 j 알파벳의 경우 베이스라인이 존재하기에 밑에 내용이 채워질 수 있음

- a 태그 : 개발시 클릭했을때 안의 내용이 없는 경우에 아무런 조치도 취하지 않을 경우에 사용
- inline 요소임
- javascript:void(0)

## css
- position: absolute; 사용시 요소의 성질이 block으로 자동으로 바뀜



## 배치
- 수직 가운데 배치하기 위해서 사용하는 코드
``` css
  top: 0;
  bottom: 0;
  margin: auto;
```

- 수직의 내용들을 수평으로 나열할때 사용하는 코드
``` css
display: flex; 
```


## 가상요소선택자
- inline요소
``` css
header .sub-menu ul.menu li::before
```

## script defer
- <script> 태그의 defer 속성은 페이지가 모두 로드된 후에 해당 외부 스크립트가 실행됨을 명시

## class 명이 띄어쓰기가 들어가있는 경우
- classList.add 를 통해서 class를 추가해주는 경우에
- 기존 클래스명에 새롭게 추가된 클래스명이 추가 됨으로서 길어지는데
- css 를 통해서 해당 내용에 수정을 가하고 싶을때
- 일치를 위해서 붙여서 쓰도록 한다 .search.focused
``` css
header .sub-menu .search.focused .material-icons-outlined{
  opacity: 0;
}
```

## transition
- all 이 default임


## 헤더와 드롭메뉴
- top이나 bottom 속성을 사용하지 않아 수직 위치 값이 없다면
- 요소의 원래 위치를 그대로 사용
- 만약 position: absolute; 를 사용했다면,
- (위치상) 부모 요소를 기준으로 하므로,
- 화면의 뷰포트 좌우 끝까지 늘어날 수 없게 됨

## BEM
- HTML 클래스 속성의 작명법
- block element modifier
- 요소__일부분 : underscore(lodash) 기호로 요소의 일부분을 표시
- 요소--상태 : Hyphen(Dash) 기호로 요소의 상태를 표시

## lodash cdn
- scrollY 사용

## gsap cdn
- js animation
```javascript
gsap.to(요소, 지속시간, 옵션);
```
- gsap -> opacity : 시각적으로만 사라진 것, 마우스 포인터로 클릭이 가능함(문제)
- gsap easing : esseInOut: power1 으로 요소의 in, out 특성에 맞는 에니메이션 적용하기
```javascript
TweenMax.to(
graph
graph, 
2.5
2.5, { ease: 
Power1.
easeInOut
easeInOut, y: -500 });
```

## 정렬
- justify-content: flex-end; 오른쪽 정렬
- align-items: center; 글자 수평 수직 가운데로 정렬

## swiper js
- 6 version vs 8 version
- current : v8.4.3 
- hw 가속 전환과 여러 기본 동작을 갖춘 현대적인 슬라이드 라이브러리
- 7,8 버전의 사용법이 다르기 떄문에 6버전으로 유지
- 첫번째 div 태그에 swiper-container 라고 시작
- 공지사항을 슬라이드로 볼 수 있게하기 위해 사용
- min~ : 원본이 아닌, 최적화된 코드, minify의 약자
- 자동플레이 및 마지막 요소에서 다시 처음으로 돌아갈 수 있게 하는 방법
```css
  autoplay: true,
  loop: true
```

## js
- new
- 생성자

# overflow: hidden;
- 요소의 크기가 줄어들면서, 그 영역 밖으로 넘치지 않도록
- 잘려서 안보이게 하기 위함

# 수평으로 만들고, 가로 너비 넘길때 줄 바꿈 허용하는 코드
```css
.rewards .btn-group {
  width: 250px;
  display: flex;
  flex-wrap: wrap;
}
```

## flex-grow: 1;
- 최대한의 너비 사용하기

## padding-top
- padding은 상대적 요소로, 늘어날 수 있는 여지를 주게 되는데
- 예를 들어, width는 500px 이고, height 을 0으로 지정해준  상태에서
- padding-top: 50% 를 설정해주게 되면, 
- 250px 으로 맞춰지게 된다 (부모요소의 가로 너비를 가져감)
- 영상 같은 곳에서 활용된다
- 보통 16: 9 의 비율을 맞추려는 경우
- 56.25 % 를 맞춰주면 된다
- fhd : 1920 x 1080


## 가상요소 선택자 ::
- .youtube .youtube__area::before 
- 가상요소 선택자에서 before을 이용하여,
- 실제 html을 건들지 않고서도, 
- css로 html 요소의 내용을 수정하는 방법

## youtube iframe api
- https://developers.google.com/youtube/iframe_api_reference?hl=ko
- var 요즘 잘 활용하지 않는 요소 생성 방법
- 요즘엔 let , const

# scrollMagic cdn
- https://nykim.work/30
- 외부 라이브러리, 스크롤 애니메이션 구현 가능
- 웹퍼블리싱에서 완성도 높이기 위해,gsap과 함께 많이 사용됨

# 특수문자
- 표현하는 방법 관련 참고 : https://www.reilldesign.com/tutorials/character-entity-reference-chart.html


# img
```css
display:block;
margin:0 auto;
```
- 위의 경우에는 width 속성이 없이도 가운데 정렬이 가능

# gsap ScrollToPlugin 
- 3.11 버전에서는 window 의 scrollTo 옵션이 정상적으로 작동하지 않음
- 대신, 3.10 버전으로 실행
## 부족한 점
- awards
-- arrow 버튼 슬라이드 요소 관리 5개 표시만 하고 싶은데 불가
-- 버튼 안보임