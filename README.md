# TechBridge Minjae Homework Branch.

## 1주차 숙제 코멘트

- `<div class="learn-more">`를 `<div class="learn more">`로 한거 이외엔 별 문제 없었습니다. 후자는 `learn`클래스와 `more`클래스가 따로 달린거라서 `learn-more`하곤 전혀 다른 클래스 입니다.

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
