### CSS의 속성 경합 

* CSS에는 여러가지 경합되는 속성이 있을 수 있음. 
* 여러가지 스타일 정보를 기반으로 **경쟁** 에 의해 가장 적절한 스타일이 반영됨

#### 선언 방식에 따른 우선순위 

> Inline -> Internal -> External

* 동일한 속성이라면 나중 속성이 선택됨. 
* 구체적인 속성 명시가 되어있는 속성이 선택됨.

e.g.

```css
body > span {
    color: red;
}

span {
    color: blue;
}

Body까지 명시한 red가 적용됨.
```

* ID가 클래스에 우선함. 

```css
#a {
    color: red;
}

.a {
    color: blue;
}
```
*빨간색으로 들어간다.* **id -> class -> element 순위임.**

> CSS Specificity로 검색해보자.