## Insert & Resize background_image ##
배경 이미지 삽입 및 크기 조정

### Resolution
1. 배경을 지정할 block 태그 생성
~~~
<div class="cover">

</div>
~~~
![url](./img/1.png)

2. html, body 세로 늘리기
~~~
html, body{
    height: 100%;
}
~~~
![url](./img/2.png)
![url](./img/3.png)

3. 전체 테두리, 여백제거
~~~
*{
    margin: 0;
    padding: 0;
    outline: 0;
}
~~~
![url](./img/4.png)

4. 배경삽입 영역 세로 늘리기
~~~
.cover{
  height: 100%;
}
~~~
![url](./img/5.png)

5. 배경 이미지 삽입
~~~
background-image: url('./img/cover_image.jpg');
~~~
![url](./img/6.png)

6. 배경 이미지 비율조정
~~~
background-size: cover;
~~~~
![url](./img/7.png)

7. 배경 이미지 위치 중앙정렬
~~~
background-position: center;
~~~
![url](./img/8.png)
