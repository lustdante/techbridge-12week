# 5주차 숙제

## Practice 9

- (1) `main`안에 `h1`, `p`, `a.btn`를 써서 제목, 문구, 그리고 링크를 만들어주세요.
  + 제목: `MOVE`
  + 문구: `Form healthy habits to take your fitness to the next level.`
  + 버튼: `START NOW`

- (2) `main`에 관련된 태그들에게 다음과 같은 스타일들을 적용해주세요.
  + 배경사진: `https://s3.amazonaws.com/codecademy-content/projects/move/bg.jpg`
  + `h1`과 `p`는 하얗게

- (3) `.main .btn`은 다음과 같이 버튼을 만들어 주세요.
  + 배경색 `#1c1c1c`
  + 글씨는 하얗게
  + 폰트크기는 18픽셀
  + 패딩은 위아래 8픽셀, 양옆 30픽셀
  + 밑줄은 빼주기

- (4) 어라? 뭐가 좀 이상하네요. 위에 있는 공백을 `.main h1`의 마진을 0으로 맞춰서 없애줍니다.

- (5) `main`안에 있는 내용이 좀 붕 떴네요. `main`의 탑 패딩에 100픽셀을 줘서 내려봅시다.

- (6) 어, 이거 `main`이 600픽셀이여야 하는데 패딩을 줘서 700픽셀로 변해버렸네요. box-sizing: border-box를 모든 태그에 적용하면 패딩이 있더라도 높이를 유지할 수 있어요! 다음 css를 파일 맨 위에 넣어주세요

```css
* {
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}
```

> 참고로 부트스트랩을 쓰면 border-box가 기본으로 적용되어있습니다.

- (7) `supporting`안에 배경색을 `#1c1c1c`으로 바꿔주세요. 그리고 `Move`처럼 말고 다음과 같은 요소들을 넣어주세요.
  + `SYNC`: `Access your activity on your phone, tablet, or computer.`
  + `COMPETE`: `Set personal challenges and see how you rank against your friends.`

> 여기서 `col`에다가 `-md-4`안달아주셔도 되요. 이건 부트스트랩이 아니라 따로 만든 예제입니다.

- (8) `feature`안에 `Move. Rest. Recover. Move.`가 들어간 `h2`를 넣어주세요.

- (9) `feature`안에 다음과 같은 스타일들을 적용해주세요.
  + 배경사진: `https://s3.amazonaws.com/codecademy-content/projects/move/feature.jpg`

> h2엔 스타일이 이미 적용되있습니다.

- (10) `feature`안에 있는 `h2`가 또 붕떠보이죠? 패딩을 이용해서 200픽셀 내려줍시다. 이미 border-box를 적용했으니 정상적으로 작동할꺼에요.

- (11) `feature`아래에 또 `supporting`을 추가해서 `h2`, `p`, `a.btn`을 넣어줍니다.
  + 부제목: `GO PREMIUM`
  + 문구: `Receive recommendations based on your activity to level up.`
  + 버튼: `LEARN MORE`

- (12) 마지막에 `footer`를 추가해서 `h2`와 `a.btn`을 넣어줍니다.
  + 배경사진: https://s3.amazonaws.com/codecademy-content/projects/move/footer.jpg
  + 부제목: `STOP SCROLLING. START MOVING`
  + 버튼: `START NOW`

- (13) `footer`에 있는 `a.btn`도 똑같이 적용해보세요. 그리고 패딩을 이용해 200픽셀 내려주세요.

- (14) 마지막으로 모든 버튼에 마우스를 올려놓으면 배경색은 `#ffa800`, 글색은 하얀색으로 변하게 만들어주세요.

> :hover라는 selector를 사용하면 됩니다. 그 코드를 위해 따로 자리를 둔게 아니니 그냥 아무대나 추가히시면 됩니다.

## Practice 10

- (1) `main`에 배경사진을 넣어주세요.
  + `https://s3.amazonaws.com/codecademy-content/projects/shutterbugg/intro.jpg`

- (2) `main`안에 제목, 문구, 그리고 링크를 넣어주세요.
  + `h1`: Introducing Shutterbugg
  + `p`: Capture the moments that matter.
  + `a.btn`: Download Shutterbugg

- (3) `main`안에 있는 `btn`을 예쁘게 꾸며봅시다.
  + 배경색: rgba(238, 68, 95, 0.9)
  + 글씨: 흰색
  + border-radius: 4px
  + 패딩: 위아래 8픽셀, 양옆 30픽셀
  + 버튼 hover시 다음과 같은 스타일을 추가
    + 배경색: rgba(238, 68, 95, 1)
    + 글씨: 흰색
    + 밑줄 제거

> rbga에서 마지막 a는 알파값 (투명도) 입니다. 밑줄은 이미 부트스트랩에서 제거 해줍니다.

- (4) `main`안에 있는 `btn`에 재미있는 효과를 추가해봅시다. 적용해보기 전과 후에 마우스를 올려서 결과를 확인해주세요.
  + 버튼엔 `transition: box-shadow 0.5s`를 추가
  + 버튼 호버에는 `box-shadow: 0px 1px 6px rgba(0, 0, 0, 0.6)`와 `transition: box-shadow 0.25s`를 추가
  + 두가지가 완성되면 마우스를 올려보기

> transition은 간단한 애니메이션 효과를 담당합니다. 여기서 box-shadow라는 값에 트렌시션을 0.5초동안 적용하라는 의미입니다. 자세한건 구글에서 검색해보세요.

- (5) 첫 `section`안에 `row`와 `col-md-6`를 써서 다음과 같은 정보를 입력합니다.
  + 왼쪽
    + 이미지: `https://s3.amazonaws.com/codecademy-content/projects/shutterbugg/share.png`
  + 오른쪽:
    + `h1`: `Share`
    + `p`: `Share your moments with the people who matter to you most. With Shutterbugg, it's easy to share with the right people.`


- (6) 두번째 `section`안에도 다음 정보들을 입력해주세요.
  + 왼쪽
    + `h1`: `Explore`
    + `p`: `Explore moments from your friends and family. Shutterbugg makes it easy to see what's happening in the world and take in everything around you.`
  + 오른쪽
    + 이미지: `https://s3.amazonaws.com/codecademy-content/projects/shutterbugg/explore.png`

- (7) (심화) 오른쪽 이미지를 무슨 수를 쓰더라도 오른쪽 정렬시켜주세요.

> 힌트1: text-align: right를 쓰면 이미지도 정렬됩니다. 하지만 img가 아니라 img를 가지고 있는 부모에게 적용해야합니다.
> 힌트2: css만으로 적용하기 힘들수도 있습니다. 새로운 클래스를 추가하거나 html안에 style 속성을 넣어서 적용해주세요.

- (8) 세번에 `section`도 다음 정보들을 입력해주세요.
  + 왼쪽:
    + 이미지: `https://s3.amazonaws.com/codecademy-content/projects/shutterbugg/save.png`
  + 오른쪽:
    + `h1`: `Save`
    + `p`: `Save every photo you take. Shutterbugg automatically saves your photos so you can show them off from anywhere.`

- (9) 마지막 `footer`엔 `col` 3개에 다음과 같은 정보를 넣어주세요. 물론 값은 4로 해야겠죠.
  + 왼쪽:
    + `h1`: `Company`
    + `ul`, `li`: `Careers`, `Terms`, `Help`
  + 왼쪽:
    + `h1`: `Company`
    + `ul`, `li`: `Careers`, `Terms`, `Help`
  + 왼쪽:
    + `h1`: `Company`
    + `ul`, `li`: `Careers`, `Terms`, `Help`
