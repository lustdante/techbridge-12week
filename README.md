# TechBridge Kiseong Homework Branch.

## 8주차 숙제 코멘트

- `row`를 두개 만드는게 아니라 하나의 `row`안에 4:8로 만드셔야 합니다.

```html
<!-- 변경 전 -->
<div class="row">
 <div class="col-md-4">
   <h1>Kimkiseong</h1>
 </div>
</div>             
<div class="row">
 <div class="col-md-8">
   <ul class="nav nav-pills" >
     <li class="active"><a>All</a></li>
     <li><a>Consumer</a></li>
     <li><a>Mobile</a></li>
     <li><a>Commerce</a></li>
     <li><a>Enterprise</a></li>             
   </ul>  
 </div>
</div>
<!-- 변경 후 -->
<div class="row">
  <div class="col-md-4">
    <h1>Kimkiseong</h1>
  </div>
  <div class="col-md-8">
    <ul class="nav nav-pills" >
      <li class="active"><a>All</a></li>
      <li><a>Consumer</a></li>
      <li><a>Mobile</a></li>
      <li><a>Commerce</a></li>
      <li><a>Enterprise</a></li>             
    </ul>  
  </div>
</div>
```

- `footer`에도 같은 실수를 하셨습니다.

- `p`스타일은 `.p`가 아니라 그냥 `p`입니다.

수고하셨습니다!

## 7주차 숙제 코멘트
### 숙제 13

- 완벽하게 하셨습니다!

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

- css에 `{}` 괄호 닫는거 잊지 마세요. 안그러면 스타일 전부 다 깨집니다.

- 배경사진 넣을때 `no-repeat center center`와 `background-size`를 잊지 말아주세요.



## 6주차 숙제 코멘트
### 숙제 11

- 두개가 아닌 하나의 `row`안에 `col-md-4`와 `col-md-8`를 넣으셔야 합니다.

```html
<!-- 변겅 전 -->
<div class="row">
 <div class="col-md-4">
   <h1>BestBite</h1>
 </div>
</div>             
<div class="row">
 <div class="col-md-8">
   <ul class="nav nav-pills" >
     <a><li class="active">About</li></a>
     <a><li>Sign Up</li></a>
     <a><li>Log in</li></a>
   </ul>  
 </div>
</div>
<!-- 변경 후 -->
<div class="row">
  <div class="col-md-4">
    <h1>BestBite</h1>
  </div>
  <div class="col-md-8">
    <ul class="nav nav-pills" >
      <a><li class="active">About</li></a>
      <a><li>Sign Up</li></a>
      <a><li>Log in</li></a>
    </ul>  
  </div>
</div>
```

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

- `jumbotron`의 배경사진에 `no-repeat center center`와 `background-size: cover;` 넣는거 잊지마세요.

- 문구를 145픽셀 내리려면 이렇게 하면 됩니다. 그리고 마진을 없앰으로서 하얀 간격을 없앨 수 있습니다.

```css
.jumbotron {
  padding-top: 145px;
  margin-bottom: 0px;
}
```

- `banner`안에 있는 `h3`에 스타일 적용하는건 그냥 스킵하셨네요. 설명이 너무 어려웠나요?

```css
.banner h3 {
  font-size: 30px;
  margin: 0;
  padding: 0;
}
```

- 부트스트랩 버튼 스타일 default와 lg는 `btn btn-lg btn-default`이거 말하는 겁니다.

- `.section.banner`안에 있는 `a`에 또 `calss` 오타내셨습니다.

- 마진을 이용해서 버튼과 간격을 내려면 `margin-bottom`이 아니라 `margin-top`을 써야 합니다.

- `page-header`다음에 넣으라고 했는데 `page-header` 안에 넣었네요.

```html
<!-- 변경 전 -->
<div class="container">
  <div class="page-header">
    <h3>Newest Contributions</h3>
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

- 사소한거지만 `section`에 있는 `h4`의 탑 마진은 30픽셀입니다.

- `scetion`라고 오타냈습니다.

> 코드를 넣었는데 적용되지 않았으면 그냥 넘어가지 말고 왜 안됬는지 확인해보세요.

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

## 5주차 숙제 코멘트
### 숙제 9

- `main`와 `feature`에 적용된 배경사진에 `no-repeat center center` 넣는거 잊지마세요. 설명은 4주체를 참조하세요.

- `feature`아래에 `supporting`을 추가하는거지 안에 추가하는게 아닙니다.

```html
<!-- 변경전 -->
<div class="feature">
      <h2>Move. Rest. Recover. Move.</h2>
    <div class="supporting">
      <h2>GO PREMIUM</h2>
      <p>Receive recommendations based on your activity to level up</p>
      <a class="btn" href="#">LEARN MORE</a>
     </div>
  <div class="container">
<div class="footer">
      <h2>STOP SCROLLING. START MOVING</h2>
      <a class="btn" href="#">START NOW</a>       

</div>


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
    <p>Receive recommendations based on your activity to level up</p>
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

`container`는 그냥 습관적으로 넣어주세요.

- `footer`도 패딩을 위 예제처럼 패딩을 이용해서 내리지 않았습니다. `main`에 하셨던것처럼 padding-top을 주거나 `feature h2`에 padding-top을 주신것처럼 하면 됩니다.

### 숙제 10

- 배경사진 `no-repeat center center`로 해주세요!

- `.btn:hover`에 `;`추가하시는것을 잊었습니다. 이거 하나로 스타일이 아예 적용이 되지 않는다는걸 잊지 마세요.

- 마지막에 `row`를 3개 추가하셨는데 `row`하나에 `col`이 여러개 들어간다는것을 잊지 말아주세요!

## 4주차 숙제 코멘트

- 배경사진 적용할때 설명에 나와있듯이

```css
/* 변경 전 */
.header {
  background-image: url(https://s3.amazonaws.com/codecademy-content/projects/innovation-cloud/bg.jpg);/* 배경화면은 여기 */
	background-size: cover;
	background-repeat: no-repeat;
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

- 이미 추가하실때 이상한 따옴표가 들어가서 이미지가 적용이 정상으로 되지 않았습니다. 항상 쌍따옴표를 사용해주세요.

- `jumbotron`에 class가 calss로 되있습니다.

- `jumbotron`안에 배경사진도 `no-repeat center center`를 꼭 써주세요.

- `.main img`안에 margin-right 오타나셨네요.

- `jumbotron`을 추가하셨을땐 `container`를 넣으셨는데 `footer`를 추가하셨을땐 `container`를 안넣으셨네요. 앞으로 `container`는 그냥 습관처럼 넣어주세요!

- `footer`에 80픽셀은 폰트 크기가 아니라 높이입니다.

```css
/* 변경 전 */
.footer {
	background-color: black;
	font-size: 80px;
	}/* 여기엔 footer의 스타일을 적용합니다. */

/* 변경 후 */
.footer {
	background-color: black;
	height: 80px;
}
```

## 3주차 숙제 코멘트

- 5번째 숙제는 완벽

- 6번째도 민재랑 같은 실수를 하셨네요.

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

- 숙제 7에선 사소하긴 하지만

```html
<div class="jumbotron">
  <div class="container">
    <h1>소아 청소년의 올바른 성장과 자세에 대한 정보를 제공한다</h1>
      <p>온라인 및 오프라인의 무분별한 성장 치료 및 관리에 대한 허점과 오류를 수정하고,
         정형외과 의사의 입장에서 성장에 필요하며, 도움이 되는 정보와 검사 및 치료가 가능한
         병원의 정보를 함게 제공한다
      </p>
  </div>
</div>
```

`h1`과 `p`은 같은 깊이에 있어서

```html
<div class="jumbotron">
  <div class="container">
    <h1>소아 청소년의 올바른 성장과 자세에 대한 정보를 제공한다</h1>
    <p>
      온라인 및 오프라인의 무분별한 성장 치료 및 관리에 대한 허점과 오류를 수정하고, 정형외과 의사의 입장에서 성장에 필요하며, 도움이 되는 정보와 검사 및 치료가 가능한 병원의 정보를 함게 제공한다
    </p>
  </div>
</div>
```

이런식으로 정렬하는게 더 가독성이 좋습니다.

또한

```html
<div class="jumbotron">
  <div class="container">
    <h1>소아 청소년의 올바른 성장과 자세에 대한 정보를 제공한다</h1>
    <p>
      온라인 및 오프라인의 무분별한 성장 치료 및 관리에 대한 허점과 오류를 수정하고,
      정형외과 의사의 입장에서 성장에 필요하며, 도움이 되는 정보와 검사 및 치료가 가능한
      병원의 정보를 함게 제공한다
    </p>
  </div>
</div>
    <div class="learn-more"> ... </div>
```

여기도 틀리진 않았지만 `jumbotron`과 `learn-more`은 같은 깊이에 있으므로

```html
<div class="jumbotron">
  <div class="container">
    <h1>소아 청소년의 올바른 성장과 자세에 대한 정보를 제공한다</h1>
    <p>
      온라인 및 오프라인의 무분별한 성장 치료 및 관리에 대한 허점과 오류를 수정하고,
      정형외과 의사의 입장에서 성장에 필요하며, 도움이 되는 정보와 검사 및 치료가 가능한
      병원의 정보를 함게 제공한다
    </p>
  </div>
</div>
<div class="learn-more"> ... </div>
```

이게 더 자연스럽습니다. **중간에서 이걸 지켜주지 않으면 그 밑에 있는 모든 정령이 다 엉망진창이 됩니다.**

- 그리고 `div.row`에서 `div`는 태그고 `.row`는 클래스라서

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

## 2주차 숙제 코멘트

- 어라, 민재랑 답지가 아주 똑같네요 ㅠㅠ

민재랑 똑같은 코멘트입니다.

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

- `<P>환자들에게 행복을 주는 정형외과 의사 김기성입니다</p>` 절때 태그는 대문자로 쓰지 않습니다.

- 설명이 부실했던것 같습니다.

```html
<div class="container">
  <h3>특징</h3>
   <p>치료를 받고자 하는 과를 검색하고 필요하면 분과도 함께 검색 가능함</p>
  <h3>카테고리</h3>
   <p>대학병원과 준종합병원 개인병원 의원등 규모별 sorting 검색 가능</p>
  <h3>추가기능</h3>
   <p>예약 기능 및 이용 후기등을 함께 볼수 있음</p>
</div>
```

이렇게가 아니라

```html
<div class="container">
  <div>
    <h3>특징</h3>
    <p>치료를 받고자 하는 과를 검색하고 필요하면 분과도 함께 검색 가능함</p>
  </div>
  <div>
    <h3>카테고리</h3>
    <p>대학병원과 준종합병원 개인병원 의원등 규모별 sorting 검색 가능</p>
  </div>
  <div>
    <h3>추가기능</h3>
    <p>예약 기능 및 이용 후기등을 함께 볼수 있음</p>
  </div>
</div>
```

이렇게 입니다.
