# CSS의 Margin, Padding

## 1. 개념
두 속성은 모두 공간을 만들지만 테두리를 기준으로 위치가 다름.
* **Margin** (바깥쪽 여백): 요소와 요소 사이의 간격 만듦. (테두리 밖 공간)
* **Padding** (안쪽 여백): 글자나 이미지와 테두리 사이의 간격 만듦. (테두리 안 공간)

## 2. 문법
한 줄에 쓰느냐, 방향별로 쓰느냐의 차이

### 단축 속성 -- 시계 방향 원칙!!
```css
.box {
/* 상하좌우 모두 20px */
  margin: 20px;

  /* 상하 10px / 좌우 20px */
  margin: 10px 20px;

  /* 상 10px / 좌우 20px / 하 30px */
  margin: 10px 20px 30px;

  /* 상 10px / 우 20px / 하 30px / 좌 40px (시계방향) */
  margin: 10px 20px 30px 40px;
}
```
### 개별 속성
특정 방향만 조절하고 싶을 때 사용
* `margin-top`, `margin-right`, `margin-bottom`, `margin-left`
* `padding-top`, `padding-right`, `padding-bottom`, `padding-left`

## 3. 주요 기능
### **Margin** : 가운데 정렬
블록 요소(div...)를 부모 요소 내에서 가운데 정렬하고 싶을 때 auto 값 사용.

```css
.container {
  width: 500px;
  margin: 0 auto; /* 상하는 0, 좌우는 자동으로 가운데 정렬 */
}
```
### **padding** : 클릭 영역 확장
버튼 만들 때 글자에 딱 붙게 만들어지지 않도록 `padding` 을 적으면 테두리 안쪽 공간이 생겨 클릭하기 편해짐.
**주의!!** padding을 적으면 전체 박스 크기가 커짐! 
          싫다면 아래 코드를 입력해 커지지 않도록 함.
```css
* {
  box-sizing: border-box; 
}
```

## 4. 사용 팁
* 배경 색이 있을 때, 글자나 이미지를 감싸는 안쪽 공간이 필요하면 `padding`
* 박스들끼리 너무 붙어있어 간격 필요하면 `margin`
* 테두리가 있어 안쪽이 답답해 보이면 `padding`, 바깥쪽이 답답해 보이면 `margin` 사용

## 5. 그 외 자료
[MDN 박스 모델 설명](https://developer.mozilla.org/ko/docs/Learn_web_development/Core/Styling_basics/Box_model)