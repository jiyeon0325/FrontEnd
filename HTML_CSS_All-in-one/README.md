## 코딩애플 강의
# HTML/CSS All-in-one 

### 이미지 가운데 정렬
display: block;   <--- 가로행을 모두 차지 </br>
margin-left: auto; </br>
margin-right: auto </br>
```
.pic {
  style="display:block;
  margin-left:auto; 
  margin-right:auto"
}
```
### 글자 가운데 정렬
text-align: center
```
.title {
  text-align: center;
}
```
### div, p, h 가운데 정렬
#### display: block 이 기본으로 있음
margin-left: auto; </br>
margin-right: auto </br>
```
.box {
  margin-left: auto;
  margin-right: auto:
}
```
### 박스 가로로 여러개 배치 (왼쪽 정렬)
float: left 
clear: both
```
<div class="container">
  <div class="header"></div>
  <div class="left-menu"></div>
  <div class="right"></div>
  <div class="footer"></div>
</div>
```
```
.container {
    width: 800px;
}

.header {
    width: 100%;    /*부모 width의 100% */
    height: 50px;
    background-color: aquamarine;
}

.left-menu {
    width: 20%;
    height: 400px;
    background-color: cornflowerblue;
    float: left;    /*왼쪽 정렬*/
}

.right {
    width: 80%;
    height: 400px;
    background-color: coral;
    float: left;     /*왼쪽 정렬*/
}

.footer {
    width: 100%;
    height: 50px;
    background-color: goldenrod;
    clear: both;    /*float 쓰고 나서 다음에 오는 요소에는 clear를 써줘야 화면에 보임*/
}
```
