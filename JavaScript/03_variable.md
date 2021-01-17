# Variable (변수)
- 변수 선언 방법
- Semantic - 의미를 부여하여 변수이름 작성

<br>

## 변수 선언과 할당
------------------
<br>

변수 선언

```javascript
var book;
```
<br>

값을 변수에 할당

```javascript
var book = "책";
```
<br>

콤마로 구분해서 한문장에 다수 작성
```javascript
var book = "책", point = 123;
```
<br>

줄 바꾸어 작성
```javascript
var book = "책", 
    point = 123;

var book = "책" 
    , point = 123;
```
<br>

같은 값 할당
~~~javascript
var point = amount = 123;
~~~
- 권장하는 형태는 아님
- 오래된 브라우저에서 값이 연동되는 경우도 있음


