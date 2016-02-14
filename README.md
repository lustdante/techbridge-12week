# TechBridge Kiseong Homework Branch.

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
