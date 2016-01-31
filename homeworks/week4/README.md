# 4주차 숙제

## practice8.html

> practice8.html와 practice8.css를 둘다 변경해야 합니다.
> 비어있어보이지만 잘 보면 밑에 내용이 있습니다.

- (1) 만들고 싶은 웹사이트입니다. [여기](https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/index.html)를 누르고 확인해주세요.
- (2) `header`안에 `h1`, `p`, `a`를 써서 제목, 문구, 그리고 링크를 만들어주세요. `a`태그 안에는 `btn`클래스를 넣어주세요.

> header안이란 말은 header안에 container 안이라는 말입니다.
> Innovation Cloud, CONNECT YOUR IDEAS GLOBALLY, Learn More
> 링크는 `<a href="#"></a>` 이렇게 해쉬태그를 넣어주세요

- (3) 버튼을 저렇게 똑같이 만들어주세요.

> 스타일할때 `.btn`에 적용해주세요

> 버튼 스타일: 하얀색 글, 검정색 바탕, 패딩, 그리고 밑줄 없애기

- (4) `header`에 `https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/bg.jpg`를 써서 배경화면을 만들어주세요.

> background: url(이미지 주소) no-repeat center center;

> background-size: cover;

> h1, p의 색깔 체크!

- (5) `nav`안에 다음과 같은 다섯개의 리스트를 만들어주세요
  + Register
  + Schedule
  + Sponsors
  + About
  + Contact

> a태그 쓸 필요 없어요.

- (6) `nav`와 `nav ul li`에 스타일을 만들어주세요.

> `nav`는 검정색 배경색

> `nav ul li`는 하얀색; display: inline-block; line-height: 80px; 양옆 패딩 10픽셀;

- (7) `main`안에 `https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/cloud.svg`가 들어간 이미지를 넣어주세요.

> 이미지 태그에 width하고 height라는 속성을 각자 192하고 128로 지정해주세요.

- (8) 방금 추가한 이미지는 왼쪽으로 float하게 하고 마진을 위 아래 50픽셀, 오른쪽 80픽셀, 그리고 왼쪽 0픽셀로 해주세요.

- (9) `main`다음에 `jumbotron`구간을 만들어주세요.

> main 바로 다음에 jumbotron. 그 안엔 container

- (10) `h2`, `p`, `a.btn`을 써서 내용을 추가해주세요.

> Stay Connected, Receive weekly insights from industry insiders, Join

- (11) `header`에 한것처럼 `jumbotron`에서도 `https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/jumbotron_bg.jpg`를 배경사진을 넣어주세요.

- (12) `jumbotron`에 있는 `h2`, `p`, `.btn` 셋다 스타일을 주세요.

> 하얀색, 오른쪽 정렬. (.btn은 float: right을 써야합니다.)

- (13) 마지막으로 `jumbotron` 다음으로 `footer`를 추가해서 `p`태그를 이용해 `© Innovation Cloud Conference`를 넣습니다.

- (14) `footer`와 그 안에있는 `p`의 스타일은 다음과 같습니다.
  + `footer`는 검은 배경, 80픽셀 높이
  + `p`는 하얀색, 폰트크기 14픽셀, line-height 80픽셀

- (15) `jumbotron`과 `footer`사이에 하얀색 갭은 어떻게 없앨 수 있을까요?
