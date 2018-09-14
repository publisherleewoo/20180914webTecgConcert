## SOM 트리 -> render 트리

CSSOM트리에서 랜더트리로 들어가서 입력이 된다.


## 레이아웃 
(임시 구조. 아래와같이 W3C에서 정의되어있지는 않다.)

+ 기본흐름층(normal Flow)
+ float층
+ 절대독립층(position)


lineBox 안에 들어갈수 있다고 해서 inline형식이라고한다.

# float
float을 줄때 본인이나 부모에 width값을 주는것이 권장된다.
주지않는다면 밑으로 떨어진다.

float을 주면, 성질이 display:block 으로 바뀐다.
position을줘도 성질이 display:block으로 바뀐다.
BFC


# float해제

+ 부모에 주는방법. (css 랜더링이 2번그려지면서 자식의 높이값을들 갖고온다. 랜더링이 2번돈다는것은 비용이 든다는것이다. ) 
  + overflow:hidden과 
  + display:inline-block
  + float (비권장)
  + position층으로 absolute나 fixed
  + display:table-cell;
  + 부모에 height,width값을 주는방법도있으나 비권장
  
+ 자식에 주는방법 
   + 마지막 자식태그에 clear:both;
  

+ 부모:after{display:block; content:''; clear:both;}


+ display의 초기값은 inline이다.