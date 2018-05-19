## Change Radio_Button ##
라디오 버튼 사각형 버튼으로 변경하기

### Resoultion
1. radio button 생성
~~~
<input type="radio" name="exam">
<input type="radio" name="exam">
~~~
![url](./img/1.png)

2. label 태그로 버튼 감싸기
~~~
<label>
    <input type="radio" name="exam">
    <span>선택1</span>
</label>

<label>
    <input type="radio" name="exam">
    <span>선택2</span>
</label>
~~~
![url](./img/2.png)
![url](./img/3.png)

3. 사각형 영역 생성을 위한 span 태그 감싸기
~~~
<label>
    <input type="radio" name="exam">
    <div class="choice1 box">
        <span>선택1</span>
    </div>
</label>

<label>
    <input type="radio" name="exam">
    <div class="choice2 box">
        <span>선택2</span>
    </div>
</label>
~~~
![url](./img/4.png)
![url](./img/5.png)

4. 기본 라디오 버튼모양 제거
~~~
input[type="radio"]{
    display: none;
}
~~~
![url](./img/6.png)

5. 사각형 꾸미기
~~~
.box{
    border: 1px solid black;
    border-radius: 3px;
    width: 10%;
    padding: 10px;
    cursor: pointer;
}
~~~
![url](./img/7.png)

6. 사각형 가로정렬
~~~
display: inline-block;
~~~
![url](./img/8.png)
![url](./img/9.png)
![url](./img/10.png)

7. 전체 중앙정렬
~~~
<div class="middle">
    <label>
        <input type="radio" name="exam">
        <div class="choice1 box">
            <span>선택1</span>
        </div>
    </label>

    <label>
        <input type="radio" name="exam">
        <div class="choice2 box">
            <span>선택2</span>
        </div>
    </label>
</div>
~~~
~~~
.middle{
    text-align: center;
}
~~~
![url](./img/11.png)

8. 버튼 선택 시 배경 색 변경
~~~
input[type="radio"]:checked + .box{
    background-color: aquamarine;
}
~~~
![url](./img/12.png)
![url](./img/13.png)
