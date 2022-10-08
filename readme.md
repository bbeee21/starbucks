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