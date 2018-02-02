### CSS Selector

* HTML의 요소를 속성이나 id, class를 사용해 얻어옴.
* 3요소 : tag, id, class 

#### Tag

* Tag를 명시하면 문서 안의 동일 태그에 다 적용됨 

#### ID

* 샵으로 시작함. 
* 해당 ID가 명시된 요소에 적용됨. 
> JS와의 차이점. *같은 아이디를 쓰는 모든 요소를 다 찾아온다.*

#### 복합 사용

* element.className

* tag#id     

* , 를 기준으로 여러개를 한 번에 선택
* Space = 하위 요소를 선택, > = 자식 요소를 선택  

```html
#pobi > span
{color: red;}

<div id = "pobi">
    <div>
        <span>css doesn't reach here!</span>
    </div>
    <span>css can reach here!</span>
</div>
```

#### N번째 요소를 선택. 

property:nth-child(n)

