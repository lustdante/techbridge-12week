# 6주차 숙제

## Practice 11

- `header`안에 하나의 `row`와 4:8로 `col-md`을 추가해주세요.

- 왼쪽 `col`엔 `BestBite`라는 문구가 달린 `h1`를 넣어주세요.

- 오른쪽 `col`엔 `ul.nav.nav-pills`를 추가해서 다음과 같은 링크 리스트들을 걸어주세요. (`li`와 `a`가 들어가있는 리스트입니다.)
  + `About`
  + `Sign Up`
  + `Log in`

> `ul.nav.nav-pills`란 `ul`이란 태그에 `nav`와 `nav-pills` 클래스가 두개 달린걸 일컫습니다.

- `About`이 들어간 `li`는 `.active`를 추가해주세요.

- `header`안에 들어간 요소들에게 다음과 같은 스타일들을 적용해주세요.
  + `.nav`에 `float:right`를 써서 오른쪽으로 넘겨줍니다.
  + `h1`에 기본 마진이 들어가있네요. 마진과 패딩을 0으로 만들어주세요.
  + `.header`에 패딩을 40픽셀로 주세요.

- `jumbotron`안에 배경사진을 추가해주세요.
  + 사진 링크: `https://s3.amazonaws.com/codecademy-content/projects/bestbite/bg.jpg`
  + 지금쯤이면 배경사진 어떻게 넣는지 알겠죠?

- `jumbotron`안에 `row`와 `col-md-4`하나를 추가해주세요. (`col`은 하나만 있어도 됩니다.)

- `h2`를 써서 다음 문구들을 추가해주세요. (`h2`를 3개 쓰셔야 합니다.)
  + `Browse.`
  + `Create.`
  + `Share.`

- `jumbotron`안에 있는 `h2`에 다음과 같은 스타일들을 적용해주세요.
  + 글씨색 하얀색
  + 폰트 사이즈 60픽셀
  + 오른쪽 정렬
  + 마진 0

- (심화) `jumbotron`안에 문구를 무슨 수를 써서라도 위에서 간격이 145픽셀이 되게 만들어주세요.

- `jumbotron`하고 `banner`사이에 뭔가 간격이 있어보이네요. 없애주세요.

- `section.banner`안에 `h3`밑에 `Learn More`가 들어간 버튼을 만들어주세요. 부트스트랩 버튼이니까 `btn`을 잊지마세요.
  + 버튼 스타일: default
  + 버튼 크기: lg

- `banner`에 있는 `h3`를 다음과 같은 스타일을 적용해주세요.
  + 폰트 크기: 30 픽셀
  + 마진/패딩: 0 픽셀

- 버튼이 지루하네요. 버튼에도 스타일을 추가해줘요.
  + 배경색: `rgba(216, 25, 47, .5)`
  + border: 0픽셀
  + 글씨색: 하얀색
  + 마진을 이용해서 버튼과 h3의 간격을 24픽셀로 맞춰주세요.

- 다음 `section`에 있는 `page-header` 다음에 `row` 한개와 `col-md` 3개를 삼등분으로 추가해주세요. 각자 `col`안에는 `h4`와 `ul.li`를 이용해서 다음과 같은 정보를 추가해주세요.
  + 제목: `Breakfast`, 내용: `Maple French Toast`, `Rolled Oats with Berries`
  + 제목: `Dinner`, 내용: `Black Bean Stuffed Peppers`, `Pesto Pasta with Spinach`
  + 제목: `Dessert`, 내용: `German Chocolate Cake`, `Hazelnut Tiramisu`

> `.section`안에 있는 모든 내용이 중간 정렬된 이유는 `.section`에 중앙 정렬 스타일이 적용되서 입니다.

- `section`에 있는 `h4`에 다음 과 같은 스타일을 적용해주세요.
  + 색깔: #d8192f
  + 마진: 위 30픽셀, 아래 20픽셀, 양 옆 0픽셀
  + 패딩: 0
  + 폰트 크기: 20픽셀

- `section`안에 있는 `ul`도 다음과 같이 적용합시다.
  + `list-style-type: none`를 써서 동그라미를 없애주세요.
  + 마진 탑을 10픽셀
  + 패딩: 0

- `footer`에 `p` 3개를 다음 내용을 넣어서 추가해주세요.
  + `© 2014 BestBite`
  + `<a href="#">BestBite.com</a>`
  + `12 Greentree Lane, Orlando, FL`

- `footer`에 다음 스타일들을 적용해주세요.
  + 높이 100픽셀
  + 패딩: 위 40, 아래 100, 양옆 0
  + `footer`위에 있는 `section`과 간격을 80픽셀
  + 배경색: #eee
  + 폰트 크기 14픽셀

- (심화) `footer`안에 있는 내용을 클래스를 추가해도 되니까 다음 처럼 보이게 해주세요.
  + 처음 `p`는 왼쪽정렬, 두번째는 중앙정렬, 세번째는 오른쪽 정렬
  + 두번째 색깔은 `#d8192f`

## Practice 12

한번 배경에 동영상을 넣어볼까요?

- `video-section`에 다음과 같은 요소를 추가해주세요.

```html
<video autoplay="" muted="" loop="">
  <source src="https://s3.amazonaws.com/codecademy-content/projects/excursion/bg.mp4" type="video/mp4">
</video>
```

> 신기하죠? 우선 html으로 내용부터 넣기로 합시다.

- `video-section`안에 `h1`과 `a.btn`을 넣어주세요. (`a`는 `p`안에 넣어주세요.)
  + 제목: `Discover hidden places in the world around you`
  + 버튼: `Download Excursion`

- 그 다음 `text-section`에는 `h2`와 `p`를 넣어주세요.
  + 부제목: `Your personal travel guide`
  + 내용: `Excursion remembers places you like, and recommends new points of interest around you.`

- `feature-section` 다음에 있는 `text-section`에 `img`, `h2`, 와 `a.btn`을 넣어주세요. (`img`는 `p`안에 넣어주세요.)
  + 이미지 링크: `https://s3.amazonaws.com/codecademy-content/projects/excursion/binoculars.png`
  + 부제목: `Available for iPhone and Android`
  + 버튼: `Download Excursion`

- `footer`에 `p`를 넣어주세요.
  + 내용: `© Excursion`

> 먼저 html부터 완성 한 다음에 스타일을 적용하는게 더 효율적입니다. 앞으론 그렇게 해주세요.

- 버튼 스타일을 다음처럼 해주세요.
  + 배경색: `#4386fc`
  + 폰트크기: 16픽셀
  + 폰트굵기: 300
  + 패딩: 위 아래 16픽셀, 양 옆 26픽셀
  + 밑줄 삭제

- `video-section`에 있는 `h1`은 다음처럼 해주세요.
  + 흰색
  + 마진: 위 0, 아래 50픽셀

- `text-section`에 있는 `h2`의 위 아래 마진을 40픽셀로 해주세요.

- `feature-section`에 배경사진 추가해주세요.
  + 사진 링크: `https://s3.amazonaws.com/codecademy-content/projects/excursion/camp.png`

- `footer`
  + 배경색: #eee
  + 폰트 크기: 11픽셀
  + 위 아래 패딩: 5픽셀, 양 옆 픽셀: 0픽셀
