# 7주차 숙제

## Practice 13

자 이제 회원가입 페이지를 만들어봅시다. 먼저 html부터 완성시켜볼까요?

- `header`안에 `img`를 넣어주세요.
  + 이미지 주소: `https://s3.amazonaws.com/codecademy-content/projects/pocketbook/logo.svg`
  + 이미지 너비: 50픽셀

- `main`안에 `row`와 `col-md-7`하나를 추가해주세요.

- 그 안에 `Join Pocketbook`이 들어간 `h1`을 넣어주세요.

- 그 다음에 이런걸 넣어주세요.

```html
<form role="form">
  <div class="form-group">
    <label for="first">First name</label>
    <input type="text" class="form-control" id="first">
  </div>
  <div class="form-group">
    <label for="last">Last name</label>
    <input type="text" class="form-control" id="last">
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" class="form-control" id="email">
  </div>
  <div class="form-group">
    <label for="password">Password</label>
    <input type="password" class="form-control" id="password">
  </div>
  <button type="submit" class="btn">Create account</button>
</form>
```

> 이게 뭔진 수업시간에 설명드리겠습니다.

- `footer`엔 `ul.li`를 추가해주세요.
  + Contact
  + Help Center
  + About

자, 이제 스타일 갑니다.

- 아예 `body`에 배경사진을 넣어주세요. 잠깐! 이건 다른 배경사진과 다른 방식을 써야합니다.
  + `background-image: url(https://s3.amazonaws.com/codecademy-content/projects/pocketbook/bg.jpg)`
  + `background-size: cover`
  + `background-repeat: no-repeat`
  + 배경색: #140e07
  + 글은 하얀색

- `header`을 중앙 정렬를 해주고 마진 아래를 50픽셀로 간격을 주세요.

- `header`에 패딩 30픽셀과 `border-bottom`을 `1px solid #e5e5e5`를 적용해주세요.

- 음... 줄이 너무 긴거 같은데, 패딩과 보더를 `header`말고 그 안에 있는 `container`에 적용해주세요. 그게 더 나은 듯

- `main` 마진 위 아래를 80픽셀로 적용해주세요.

- `h1`의 크기를 30픽셀, 마진을 아래만 20픽셀, 나머지는 0으로 해주세요.

- 회원가입 버튼을 다음과 같이 적용해주세요.
  + 마진 탑은 30픽셀
  + 하얀색
  + 배경색은 rgba(0,240,190,0.25)
  + border는 0픽셀줘서 없애주세요.
  + border-radius도 0으로 해서 사각으로 해주세요.

- `footer` `container`도 위아래 패딩을 20픽셀로 두고 위 `border-bottom`한 것처럼 여긴 `border-top`을 적용해줍니다.

- `footer`에 있는 `ul`엔 다음 스타일을 적용해주세요.
  + list-style: none해서 동그라미를 없애주세요.
  + 양옆 패딩 20픽셀
  + 아래 마진 80픽셀

- `footer`에 있는 `li`엔 다음 스타일을 적용해주세요.
  + `display`: `inline`
  + 오른쪽 마진: 20픽셀

## Practice 14

뜨악, html에 아무것도 없네요. 패닉하지 말고 차근차근히 진행합시다.

- `jumbotron`과 `container`를 넣습니다.

- 그 안에 `header`와 `main`을 넣습니다.

- `header`안에는 `row`와 3:9로 `col-md`를 넣어주세요.

- 왼쪽 `col`에는 `logo.svg`를 넣어주세요. (로고는 같은 폴더에 있습니다.)
  + 너비 106, 높이 75

- 오른쪽에는 `ul.li`를 써서 다음을 넣어주세요.
  + `<a href="#">Features</a>`
  + `<a class="btn btn-default" href="#">Download</a>`

- `main`안에도 `row`와 7짜리 `col-md`한개 넣어주세요.

- 그 안에는 `h1`과 `p`를 넣어주세요.
  + 제목: `Turn Up the Bass`
  + 내용: `From the newest releases to classic albums, we have the best music for you to enjoy.`

- `jumbotron` 다음에 `supporting-1` + `container`를 추가해주세요.

- 이왕 할겸 `supporting-2` ~ `supporting-4`도 같은 방식으로 추가합니다. 미리 `container`도 넣어주세요.

- `supporting-1`에는 6:6으로 `row`와 `col-md`를 넣어주세요.

- 왼쪽엔 이미지를 넣어주세요.
  + 이미지 주소: `https://s3.amazonaws.com/codecademy-content/projects/bass/you.svg`
  + 너비 450, 높이 300

- 오른쪽엔 `h2`와 `p`를 써서 다음을 넣어주세요.
  + 부제목: `Music Just for You`
  + 내용: `Listen to your favorite artists and albums, and make playlists of your favorite songs. Get recommendations based on your tastes to discover new music.`

- `supporting-2`도 6:6으로 하는데 이번엔 오른쪽엔 콘텐트, 왼쪽엔 이미지를 넣어주세요.
  + 부제목: `Listen Everywhere`
  + 내용: `Take your music with you everywhere you go. Listen for free for free on any device - mobile, tablet, and your computer.`
  + 이미지 주소:  `https://s3.amazonaws.com/codecademy-content/projects/bass/everywhere.svg`
  + 이미지 너비 450, 높이 300

- `supporting-3`도 똑같이. 이번엔 1처럼 왼쪽은 사진, 오른쪽은 콘텐츠로 해주세요.
  + 이미지 주소: `https://s3.amazonaws.com/codecademy-content/projects/bass/connect.svg`
  + 이미지 너비 450, 높이 300
  + 부제목: `Connect with Others`
  + 내용: `Find the right songs for the right occassions. Let your friends know what you're listening to, and connect with others who share the music you love.`

- 마지막 `supporting-4`에는 `row`쓰지 말고 그냥 `h2`와 이미지 두개 넣어줍니다.
  + 부제목: `Try it now`
  + 첫 이미지 주소: `https://s3.amazonaws.com/codecademy-content/projects/bass/app-store.png`
  + 두번째 이미지 주소: `https://s3.amazonaws.com/codecademy-content/projects/bass/google-play.png`

- `footer`내용이 좀 많네요. 각오하세요. `row`와 `col-md`를 써서 2:2:2:2로 해주세요.

- 각자 `col`에는 `ul`, `li`, `a`를 써서 링크 리스트를 넣어주세요. 아, 그 `ul`의 첫 요소는 `h3`로 링크 제목을 넣어주세요.
  + 부제목: `Bass`
    + `Install`
    + `Mobile`
  + 부제목: `About`
    + `Blog`
    + `Team`
    + `Jobs`
  + 부제목: `Support`
    + `Help Center`
    + `Get Started`
    + `Contact Us`
  + 부제목: `Community`
    + `Facebook`
    + `Twitter`
    + `Google+`

휴. 힘들었죠? 이제 스타일을 적용할 시간입니다!

- `html, body`안에 추가로 배경색 `#161718`와 글씨색 하얀색을 적용합니다. 이러면 안에 있는 모든 글들이 하얀색으로 적용됩니다. (a는 예외)

- `jumbotron` 높이를 560픽셀로 해주고 배경사진을 넣어줍니다.
  + 이미지 링크: `https://s3.amazonaws.com/codecademy-content/projects/bass/bg.jpg`

- `header`안에 있는 `a`를 하얗게 해주세요. 그리고 패딩 15픽셀과 두껍게 해주세요.

- `header`안에 있는 `li`의 `display`를 `inline-block`을 넣어서 가로 한줄로 만들어줍시다. 아 그리고 왼쪽 마진은 13픽셀, 위 마진은 40픽셀 주세요.

- `header`안에 있는 버튼을 다음을 적용해줍니다.
  + 보더 없애주세요.
  + 버튼을 사각으로 해주세요.
  + 위 아래 패딩은 8픽셀, 양옆은 30픽셀
  + 배경색은 `#ff003d`

- `main`에 있는 `h1` 위에 간격을 60픽셀로 어떻게든 두세요.

- `supporting-1`부터 `supporting-4`까지 전부 위아래 패딩 70픽셀, 양옆 30픽셀을 주세요.

- `supporting-2` 배경색은 검은색으로 해주세요.

- `supporting-4`를 중앙 정렬과 높이 400픽셀로 맞추고 배경사진을 추가해주세요.
  + 이미지 링크: `https://s3.amazonaws.com/codecademy-content/projects/bass/feature.jpg`

- `supporting-4`에 있는 `h2`의 위 간격을 80픽셀로 주세요.

- `footer`의 배경색은 검은색, 위 패딩 50픽셀, 아래 패딩 35픽셀, 양옆은 0픽셀

- `footer`의 `h3`는 크기를 15픽셀로 해주세요.

- `footer`안에 있는 `ul`의 패딩 0, 그리고 list-style을 none으로 해주세요.

- `footer`안에 있는 `a`는 다음 스타일들을 적용해주세요.
  + 색: `#aaa`
  + 폰트 사이즈: 13픽셀
  + 위 아래 패딩 5픽셀, 양옆은 0
  + 아, a의 `display`는 `inline`입니다. 패딩이 적용이 안되요. `inline-block`을 적용해주세요.

  ## Practice 15

  장고 프로젝트를 직접 셋팅하는 과제입니다. 예전에 사용했던 index.html과 index.css를 이용해서 간단한 서버를 구축할겁니다.

  - (1) 한번 index.html을 열어서 어떻게 생겼는제 확인해주세요.

  - (2) 만일 장고를 설치하지 않았으면 pip를 이용해서 장고를 설치해주세요. (다들 설치되있을꺼에요.)

  ```bash
  pip install django
  ```

  - (3) practice15 폴더 안에 장고 프로젝트를 만들어주세요.

  ```bash
  django-admin startproject practice11
  ```

  - (4) 장고 앱을 만들어주세요.

  ```bash
  python manage.py startapp home
  ```

  - (5) `practice11/settings.py`에 있는 `INSTALLED_APPS`에 만들었던 앱을 추가해주세요.

  ```python
  INSTALLED_APPS = [
      'django.contrib.admin',
      'django.contrib.auth',
      'django.contrib.contenttypes',
      'django.contrib.sessions',
      'django.contrib.messages',
      'django.contrib.staticfiles',
      'practice11',
  ]
  ```

  - (6) `home/views.py`에 index 뷰를 만들어주세요.

  ```Python
  from django.shortcuts import render


  def index(request):
      return render(request, "index.html", {})
  ```

  - (7) `practice11/urls.py`를 다음과 같이 변경해주세요.

  ```python
  from django.conf.urls import include, url

  urlpatterns = [
      url(r'^', include('home.urls')),
  ]
  ```

  - (8) `home/urls.py` 파일을 만들어서 다음과 같은 코드를 추가해주세요.

  ```python
  from django.conf.urls import url
  from . import views

  urlpatterns = [
      url(r'^$', views.index, name='index'),
  ]
  ```

  - (9) `practice11/home/templates/`을 만들어주고 `index.html`파일을 옮깁니다.

  - (10) `pratice11/home/static/css/`를 만들어주고 `index.css`파일을 옮깁니다.

  - (11) `manage.py`가 있는 폴더로 돌아가서 서버를 키고 한번 작동하는지 확인합니다.

  ```bash
  python manage.py runserver
  ```

  - (12) 아, 하나 빼먹었네요. `index.html`에 `index.css`를 불러오는 코드를 다음과 같이 변경해주세요. 그리고 다시 시도해보세요.

  ```html
  <!-- 파일 맨 위 -->
  {% load staticfiles %}

  <!-- css 불러왔던 곳 (아래걸로 교체) -->
  {% static 'css/index.css' %}
  ```

  - 만일 뭔가가 잘못됬으면 어떤걸 빼먹었는지 다시 한번 찾아보세요. 웹 개발은 이러한 문제를 해결할 수 있는 문제 해결 능력이 많이 요구됩니다.

  - 앞으로 장고로 프로젝트를 시작할때 이 과정을 참고하세요.
