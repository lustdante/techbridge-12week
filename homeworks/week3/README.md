# 3주차 숙제

## 과제

## practice5.html

> practice5.html와 practice5.css를 둘다 변경해야 합니다.
> 적용과 결과 확인을 문제별로 진행해주세요.

- (1) body안에 빈 div 3개를 추가해주세요.
- (2) 3개의 div안에 img태그를 넣어주세요. src 속성은 같이 첨부된 이미지를 참조하세요.
> 힌트. src="images/daniel.jpg"

- (3) div의 스타일을 가로 100px, 세로 100px, 그리고 보더를 2px solid black으로 지정해주세요.
- (4) 어, 이거 뭐 이미지가 좀 밖으로 삐져나오네요. div 안에 있는 img의 가로를 100%로 지정해주세요.
- (5) 사각형은 좀 지루하죠? 원으로 만들겠습니다. div의 border-radius를 100%로 해주세요.
- (6) 어랏, 이미지가 또 따로 노네요. 원 바깥으로 튀어나온 이미지를 감추기 위해 div의 overflow를 hidden으로 해주세요.
- (7) 자, 이제 9개 이미지를 모두 사용해서 친구 9명을 전부 추가해주세요.
- (8) 이제 친구 9명에 `friend`, `family`, 그리고 `enemy` 클래스를 추가해주세요. 꼭 3명/3명/3명으로 할 필요는 없지만 각자 카테고리에 최소 1명은 있도록 해주세요.
- (9) `friend`의 보더는 `2px dashed #008000`, `family`는 `2px dashed #0000FF`, `enemy`는 `2px dashed #FF0000`으로 지정해주세요.
- (10) 여기서 `friend`중에서 하나의 id를 `best_friend`, `enemy`중에서 하나의 id를 `archnemesis`로 지어주세요.
- (11) `#best_friend`는 `4px solid #00C957`, `#archnemesis`는 `4px solid #CC0000`로 지정해주세요.

## practice6.html

> practice6.html와 practice6.css를 둘다 변경해야 합니다.

- (1) 먼저 시작하기전에 파일을 열고 html와 css하나하나를 다 관찰하세요.
- (2) `header` 클래스의 배경색을 `#333333`로 설정해주세요.
- (3) `nav` 클래스안에 다음 메뉴들을 추가해주세요
  + 서비스 소개
  + 팀 소개
  + 연락하기
- (4) `.nav li`를 `display` 속성을 `inline-block`으로 설정해주세요.
- (4) `jumbotron` 클래스안에 배경사진을 추가해주세요.
> background-image: url(http://s3.amazonaws.com/codecademy-content/projects/broadway/bg.jpg);

- (5) 이미지가 너무 크네요. `background-size`를 `cover`로 설정해주세요.
- (6) 지금은 문제 없지만 이미지 반복을 막기 위해서 `background-repeat`를 `no-repeat`로 해주세요. (큰 변화는 없음)
- (7) 그리고 좀 재밌는 효과를 넣기 위해서 `background-attachment`를 `fixed`로 설정해주세요. 그리고 한번 스크롤을 해봐요!
- (8) `main`클래스 안에 있는 `h1`밑에 `시작하기`라는 문구가 달린 `a`태그를 추가해주세요. 아직 `src`는 필요없습니다.
- (9) 그 시작하기 태그에 `btn-main`이라는 클래스를 추가해주세요.

## practice7.html

> practice2.html 기억나시죠? 그거 복사 붙여넣기해서 practice7.html으로 시작할께요!

- (1) `practice7.css`를 만들고 `practice7.html`안에 `link`를 이용해서 추가해주세요.
- (2) 회사소개, 로그인, 회원가입을 `<a href="#">`으로 감싸주세요.
> 예제: <li><a href="#">회사소개</a></li>

- (3) `nav`클래스 안에 있는 모든 `a`태그를 다음 스타일들을 적용해주세요.
  + 색깔: #5a5a5a
  + 폰트크기: 11픽셀
  + 두껍게
  + 위 아래 패딩: 14픽셀
  + 양옆패딩: 10픽셀
  + 모두 대문자 (구글에 css uppercase로 검색)
  + display: inline-block
- (4) `jumbotron`이라는 클래스에 다음 스타일들을 적용해주세요.
  + 높이: 500픽셀
  + 배경사진: `https://goo.gl/04j7Nn`
  + 배경 반복없음
  + 배경 사이즈는 cover
- (5) `jumbotron`클래스 안에 `container` 안에 있는 `h1`에 다음 스타일들을 적용해주세요. (3단계로 해야 합니다.)
  + 하얀색
  + 폰트크기: 48픽셀
  + 두껍게
- (6) `jumbotron`클래스 안에 있는 `p`에 다음 스타일들을 적용해주세요.
  + 하얀색
  + 폰트크기: 20픽셀
- (7) `learn-more`클래스에 다음 스타일들을 적용해주세요.
  + 배경색 #f7f7f7
  + 위 패딩: 25픽셀
  + 아래 패딩: 50픽셀
- (8) `learn-more`안의 `h3`를 크기 18픽셀, 그리고 두껍게 해주세요.
- (9) `nav`안에 있는 `li`의 `display`를 `inline`으로 해주세요.
- (10) `jumbotron`안에 있는 `container`의 `position`를 `relative`로 하고 `top`을 100픽셀 주세요.
- (11) `<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">`를 추가해주세요.
- (12) `nav`안에 있는 첫 `ul`에 `pull-right`클래스를 추가합니다.
- (13) `learn-more`안에 `container`안에 있는 `div` 3개를 `div.row`로 감싸주세요.
- (14) 방금 말한 `div` 3개에 `col-md-4`라는 클래스를 넣어주세요.
