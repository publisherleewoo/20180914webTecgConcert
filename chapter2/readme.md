# 브라켓

어도비사 제품이기때문에 호환성이좋다.
디자이너가 쓰기에 좋은 툴.

# RWD(반응형 웹 디자인 Responsive Web Design)


+ ie8은 소수점 2자리부터자른다


+ 미디어쿼리는 뷰포트를 기준으로 접근

+ 모바일 퍼스틑 해놓는다면 미디어쿼리가 접근되지않는 상황에서도 화면출력이 된다



# picture 엘리먼트 
+ 적응형웹의 기술(adapive web)

https://www.html5rocks.com/ko/tutorials/responsive/picture-element/


```html
<!-- media="(min-width: 650px)" 와 같은 뷰포트에따라 변경됨. 1.5x  2x 이런것은 배율 -->

<picture>
  <source
    media="(min-width: 650px)"
    srcset="images/kitten-stretching.png,
            images/kitten-stretching@1.5x.png 1.5x,
            images/kitten-stretching@2x.png 2x">
  <source
    media="(min-width: 465px)"
    srcset="images/kitten-sitting.png,
            images/kitten-sitting@1.5x.png 1.5x
            images/kitten-sitting@2x.png 2x">
  <img
    src="images/kitten-curled.png"
    srcset="images/kitten-curled@1.5x.png 1.5x,
            images/kitten-curled@2x.png 2x"
    alt="a cute kitten">
</picture>


```