# TechBridge Minjae Homework Branch.

## 7주차 숙제 코멘트

### 숙제 13

- 완벽하게 했습니다.

### 숙제 14

- logo.svg는 어떻게 입력하셨는진 모르겠지만 그냥

```html
<img src="logo.svg" width="106" height="75">
```

이렇게 넣으면 됩니다.

- html은 다 잘하셨는데 footer에서 4번째 col-md-2에 ul를 빼먹으셨네요.

```html
<!-- 변경 전 -->
<div class="col-md-2">
    <h3>Community</h3>
        <a><li>Facebook</li></a>
        <a><li>Twitter</li></a>
        <a><li>Google+</li></a>
</div>
<!-- 변경 후 -->
<div class="col-md-2">
  <ul>
    <h3>Community</h3>
    <li><a>Facebook</a></li>
    <li><a>Twitter</a></li>
    <li><a>Google+</a></li>
  </ul>
</div>
```

아, 그러고 보니까 `li`와 `a`가 뒤섞여네요. `ul` 바로 아래는 `li`가 와야 한다는 것을 꼭 잊지 마세요!

## 6주차 숙제 코멘트

- 배경사진 넣을때 `no-repeat center center`와 `background-size`를 잊지 말아주세요.

### 숙제 11

- `ul` 안에는 무조건 `li`가 와야합니다. `a`는 `li`안에 들어갑니다.

```html
<!-- 변경 전 -->
<ul class="nav nav-pills" >
  <a><li class="active">About</li></a>
  <a><li>Sign Up</li></a>
  <a><li>Log in</li></a>
</ul>
<!-- 변경 후 -->
<ul class="nav nav-pills" >
  <li class="active"><a>About</a></li>
  <li><a>Sign Up</a></li>
  <li><a>Log in</a></li>
</ul>
```

- `header`안에 있는 요소 `.nav`, `h1`과 `.header`에 스타일 적용하시는건 따로 만드셔야 됬습니다. `@media (max-width: 680px)`는 아직 배우지 않은 부분이라서 건드시면 안됩니다.

```css
.header {
  padding: 40px;  
}

.header h1 {
  margin: 0;
  padding: 0;
}

.nav {
  float: right;
  width: 340px;
}
```

- `jumbotron`의 배경사진에 `no-repeat center center`넣는거 잊지마세요.

- 문구를 145픽셀 내리려면 이렇게 하면 됩니다. 그리고 마진을 없앰으로서 하얀 간격을 없앨 수 있습니다.

```css
.jumbotron {
  padding-top: 145px;
  margin-bottom: 0px;
}
```

- 부트스트랩 버튼 스타일 default와 lg는 `btn btn-lg btn-default`이거 말하는 겁니다.

- `<div class="section banner">`이걸 가르킬려면 `.section.banner`로 해야 합니다

```css
/* 변경 전 */
.section banner h3 {
    font-size: 30px;
    margin: 0px;
    padding: 0px;
}
/* 변경 후 */
.section.banner h3 {
    font-size: 30px;
    margin: 0px;
    padding: 0px;
}
```

- 마진을 이용해서 버튼과 간격을 내려면 `margin-bottom`이 아니라 `margin-top`을 써야 합니다.

- `page-header`다음에 넣으라고 했는데 `page-header` 안에 넣었네요.

```html
<!-- 변경 전 -->
<div class="container">
  <div class="page-header">
      <div class="row">
          <div class="col-md-4">
              <h4>Breakfast</h4>
              <ul>
                  <li>Maple French Toast</li>
                  <li>Rolled Oats with Berries</li>
              </ul>
          </div>
          <div class="col-md-4">
              <h4>Dinner</h4>
              <ul>
                  <li>Black Bean Stuffed Peppers</li>
                  <li>Pesto Pasta with Spinach</li>
              </ul>
          </div>
          <div class="col-md-4">
              <h4>Dessert</h4>
              <ul>
                  <li>German Chocolate Cake</li>
                  <li>Hazelnut Tiramisu</li>
              </ul>    
          </div>
      </div>
    <h3>Newest Contributions</h3>
  </div>

</div>
<!-- 변경 후 -->
<div class="container">
  <div class="page-header">
    <h3>Newest Contributions</h3>
  </div>
  <div class="row">
      <div class="col-md-4">
          <h4>Breakfast</h4>
          <ul>
              <li>Maple French Toast</li>
              <li>Rolled Oats with Berries</li>
          </ul>
      </div>
      <div class="col-md-4">
          <h4>Dinner</h4>
          <ul>
              <li>Black Bean Stuffed Peppers</li>
              <li>Pesto Pasta with Spinach</li>
          </ul>
      </div>
      <div class="col-md-4">
          <h4>Dessert</h4>
          <ul>
              <li>German Chocolate Cake</li>
              <li>Hazelnut Tiramisu</li>
          </ul>    
      </div>
  </div>
</div>
```

- 심화 문제는 너무 어려웠던것 같습니다.

### 숙제 12


- 아마 설명이 좀 헷갈렸을수도 있었습니다. `video`는 `section-content`안이 아니라 위에 넣는 거였습니다.

```html
<!-- 변경 전 -->
<div class="video-section">
  <div class="section-content container">
    <video autoplay="" muted="" loop="">
    <source src="https://s3.amazonaws.com/codecademy-content/projects/excursion/bg.mp4" type="video/mp4">
    </video>
    <h1>Discover hidden places in the world around you</h1>
    <p><a class="btn" href="#">Download Excursion</a></p>
  </div>
</div>
<!-- 변경 후 -->
<div class="video-section">
  <video autoplay="" muted="" loop="">
    <source src="https://s3.amazonaws.com/codecademy-content/projects/excursion/bg.mp4" type="video/mp4">
  </video>
  <div class="section-content container">
    <h1>Discover hidden places in the world around you</h1>
    <p><a class="btn" href="#">Download Excursion</a></p>
  </div>
</div>
```

- `.feature-section`에 배경사진은 `no-repeat center center`와 `background-size: cover`를 써주세요.

- `.text-section`에 `div` 닫아주는걸 잊어서 스타일이 깨졌네요.

```html
<!-- 변경 전 -->
<div class="text-section">
  <div class="container">
    <p><img class="app" src="https://s3.amazonaws.com/codecademy-content/projects/excursion/binoculars.png">
    </p>
    <h2>Available for iPhone and Android</h2> <a class="btn" href="#">Download Excursion</a> </div>
</div>
<!-- 변경 후 -->
<div class="text-section">
  <div class="container">
    <p><img class="app" src="https://s3.amazonaws.com/codecademy-content/projects/excursion/binoculars.png">
    </p>
    <h2>Available for iPhone and Android</h2> <a class="btn" href="#">Download Excursion</a> </div>
  </div>
</div>
```


## 5주차 숙제 코멘트

### 숙제 9
- 배경사진이 적용됬긴 했지만

```css
/* 변경 전 */
.main {
  background-image: url(https://s3.amazonaws.com/codecademy-content/projects/move/bg.jpg);
  background-size: cover;
}

/* 변경 후 */
.main {
  background: url(https://s3.amazonaws.com/codecademy-content/projects/move/bg.jpg) no-repeat center center;
  background-size: cover;
}
```

설명은 4주차에도 담겨있습니다.

- 11번에서 `feature` 안이 아니라 아래에 `supporting`을 추가하셔야 합니다.

```html
<!-- 변경 전 -->
<div class="feature">
    <h2>Move. Rest. Recover. Move.</h2>
        <div class="supporting">
            <h2>GO PREMIUM</h2>
            <p>Receive recommendations based on your activity to level up.</p>
            <a class="btn" href="#">LEARN MORE</a>
        <div class="footer">
            <h2>STOP SCROLLING. START MOVING</h2>
            <a class="btn" href="#">START NOW</a>
        </div>
        </div>
  <div class="container">

  </div>
</div>
<!-- 변경 후 -->
<div class="feature">
  <div class="container">
    <h2>Move. Rest. Recover. Move.</h2>
  </div>
</div>

<div class="supporting">
  <div class="container">
    <h2>GO PREMIUM</h2>
    <p>Receive recommendations based on your activity to level up.</p>
    <a class="btn" href="#">LEARN MORE</a>
  </div>
</div>


<div class="footer">
  <div class="container">
    <h2>STOP SCROLLING. START MOVING</h2>
    <a class="btn" href="#">START NOW</a>
  </div>
</div>
```

그리고 `container`는 습관적으로 추가해주세요.

- 10번에 있는 200픽셀 패딩을 `feature`가 아니라 `supporting`에 추가하셨네요. 그리고 패딩으로 내리는건 `padding-bottom`이 아니라 `padding-top`을 쓰셔서 내리는 의미였습니다.

### 숙제 10

- 앞으로 배경사진 적용할때 `no-repeat center center` 쓰는거 잊지 마세요!
- 버튼에 패딩 추가하시는거 깜빡하셨어요!

## 4주차 숙제 코멘트

- 배경사진 적용할때 설명에 나와있듯이

```css
/* 변경 전 */
.header {
  background-image: url(https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/bg.jpg);
  background-size: cover;
}
/* 변경 후 */
.header {
  background: url(https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/bg.jpg) no-repeat center center;
  background-size: cover;
}
```

이런식으로 background-image만 쓰는게 아니라 background를 써서 뒤에 `no-repeat center center`까지 적용시켜야 배경사진이 가운데 정렬로 적용됩니다. 안그러면 사진 윗부분이 적용되게 됩니다.

- 흠... 설명은 `nav`안이라고 했지만 다른 섹션들도 보면 모두 내용들이 `container` 안에 들어가있습니다. 되도록이면 내용들은 `container`안에 넣어주세요.

```html
<!-- 변경 전 -->
<div class="nav">
  <ul>
    <li>Register</li>
    <li>Schedule</li>
    <li>Sponsors</li>
    <li>About</li>
    <li>Contact</li>
      <div class="container">

      </div>
  </ul>
</div>
<!-- 변경 후 -->
<div class="nav">
  <div class="container">
    <ul>
      <li>Register</li>
      <li>Schedule</li>
      <li>Sponsors</li>
      <li>About</li>
      <li>Contact</li>
    </ul>
  </div>
</div>
```

- img에는 `background-image` 스타일을 추가할 필요가 없습니다. 보통 `background-image`은 배경사진 넣을때만 쓰지만 (7)번에 나와있는 사진은 이미지를 보여주는데 사용됩니다.

- `main`섹션에 들여쓰기 주의해주세요.
- (12) 여기 `jumbotron`에는 배경사진을 제대로 적용하셨어요!
- `jumbotron`을 추가하셨을땐 `container`를 넣으셨는데 `footer`를 추가하셨을땐 `container`를 안넣으셨네요. 앞으로 잊지 말아주세요!

## 3주차 숙제 코멘트

- 5번째 숙제는 완벽!

- 6번째 숙제에서

```html
<div class="jumbotron">
  <img src="http://s3.amazonaws.com/codecademy-content/projects/broadway/bg.jpg">
</div>
  <div class="container">
    <div class="main">
      <h1>테크브릿지</h1>
       <a class="btn-main">시작하기</a>

    </div>
  </div>
</div>
```

문제를 보면

- (4) `jumbotron` 클래스안에 배경사진을 추가해주세요.
> background-image: url(http://s3.amazonaws.com/codecademy-content/projects/broadway/bg.jpg);

이렇게 나와있는데 배경사진을 스타일로 넣지 않고 태그로 넣었네요. 위에 잘 살펴보면 태그들이 잘 닫혀있지 않은게 보일꺼에요.

```html
<div class="jumbotron"> <!-- jumbotron 열림 -->
  <img src="http://s3.amazonaws.com/codecademy-content/projects/broadway/bg.jpg">
</div> <!-- jubmotron 닫힘 -->
  <div class="container"> <!-- container 열림 -->
    <div class="main">
      <h1>테크브릿지</h1>
       <a class="btn-main">시작하기</a>

    </div>
  </div> <!-- container 닫힘 -->
</div> <!-- ????????????? -->
```

정답은 html을 이렇게 하고

```html
<div class="jumbotron">
  <div class="container">
    <div class="main">
      <h1>테크브릿지</h1>
      <a class="btn-main">시작하기</a>
    </div>
  </div>
</div>
```

css를 이렇게 합니다.

```css
.jumbotron {
  height: 800px;
  background-image: url(http://s3.amazonaws.com/codecademy-content/projects/broadway/bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment:fixed;
}
```

다시 한번 해보세요.

- 숙제 7에서

```css
.learn more {
  background-color: #f7f7f7;
  padding-top: 25px;
  padding-bottom: 50px;
}

.learn more h3 {
  font-size: 18px;
  font-weight: bold;
}
```

`.learn more` 또 실수했네요. 이러면 `.learn`클래스 안에 `more`라는 태그에 적용한다는 식으로 되버려요. `more`라는 태그는 존재하지 않아요 ㅎ

```css
.learn-more {
  background-color: #f7f7f7;
  padding-top: 25px;
  padding-bottom: 50px;
}

.learn-more h3 {
  font-size: 18px;
  font-weight: bold;
}
```

이렇게 하면 됩니다.

그리고 `div.row`에서 `div`는 태그고 `.row`는 클래스라서

```html
<div.row>
 <div class="col-md-4">
  <h3>빠른 시간</h3>
  <p>되도록 36시간 이내로 해드립니다.</p>
 </div>
 <div class="col-md-4">
  <h3>맞춤 시간표</h3>
  <p>자신의 시험 스케줄과 일과에 맞추어 맞춤 시간표를 짜드립니다.</p>
 </div>
 <div class="col-md-4">
  <h3>좋은 퀄리티</h3>
  <p>시험 계획표를 짜본 경험이 굉장히 많은 학생들이 짜드립니다.</p>
</div.row>
```

이게 아니라

```html
<div class="row">
 <div class="col-md-4">
  <h3>빠른 시간</h3>
  <p>되도록 36시간 이내로 해드립니다.</p>
 </div>
 <div class="col-md-4">
  <h3>맞춤 시간표</h3>
  <p>자신의 시험 스케줄과 일과에 맞추어 맞춤 시간표를 짜드립니다.</p>
 </div>
 <div class="col-md-4">
  <h3>좋은 퀄리티</h3>
  <p>시험 계획표를 짜본 경험이 굉장히 많은 학생들이 짜드립니다.</p>
</div>
```

이렇게 하는 겁니다.

## 2주차 숙제 코멘트

```css
p {
  color: red;
  }

/* 이건 틀리지 않았지만 가능하면 깔끔하게 하면 좋아요. */

p {
  color: red;
}
```

```css
h3 {
  font-family: Verdana;
  }
   {
  font-size: 16px;
  }
   {
  color: white;
  }

/*
이건 전혀 올바른 문법이 아닙니다. css는 항상
(셀렉터) {
  (속성): (값)
}
으로 되있어야 해서
{
font-size: 16px;
}
그냥 이렇게만 있으면 아무것도 아니게 됩니다. 정답은
*/

h3 {
  font-family: Verdana;
  font-size: 16px;
  color: white;
}

/* 이렇게 */
```

## 1주차 숙제 코멘트

- `<div class="learn-more">`를 `<div class="learn more">`로 한거 이외엔 별 문제 없었습니다. 후자는 `learn`클래스와 `more`클래스가 따로 달린거라서 `learn-more`하곤 전혀 다른 클래스 입니다.
