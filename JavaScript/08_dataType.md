# Data Type(데이터 타입)
- 자료형이라고도 함.
- Number, String, Null, Undefined, Boolean, Object

<br>

## 데이터는 타입을 가진다
--------------------
~~~javascript
var point = 123;
console.log(typeof point);
point = "책";
consolt.log(typeof point);

// Output: 
// number
// stirng
~~~
~~~java
// java
int point = 123; // int라고 선언
point = "책";
// error : Type mismatch: cannot convert from String to int
~~~
- 타입을 먼저 선언하고 타입에 맞는 데이터를 할당하는 언어(java)와 달리
- JS는 데이터를 기준으로 타입을 결정한다.

<br>

## Number 타입
---------------
- 부호(+, -)를 가진 값
- 특수한 3개 값
  - Infinity : 양수 무한대
  - -Infinity : 음수 무한대
  - NaN : Not-a-Number
  
    ~~~javascript
    var point = 1 * "A";
    console.log(point);

    // Output : NaN
    // 숫자가 아니다.
    ~~~

<br>

## String 타입
-----------------
- 값은 "" 또는 '' 사이에 작성

<br>

## undefined 타입
-----------
  - 변수의 디폴트 값 : JS에서 변수가 이름과 값을 갖는 구조를 맞추기 위한 것
    ~~~javascript
    var point;
    console.log(point);

    // Output : undefined
    ~~~
  - 변수에 undefined 할당 가능
  - But, undefined라는 값을 할당한 것인지 아니면 값을 할당하지 않은 것인지 구분이 가지 않으므로 권장 X.
  - 대신 null을 사용

<br>

## null 타입
-------------
- 값이 없다는 의미.
- 값을 할당하지 않았다는 뜻의 undefined과 차이가 있음.
  
    ~~~javascript
    var book;
    console.log(book);
    
    var point = null;
    console.log(point);
    // Output: null
    ~~~

<br>

## Boolean 타입
-------------
- 값 : true, false

<br>

## Object 타입
-------------
- {name: value} 형태
- 프로퍼티: name 과 value 하나의 쌍을 지칭
- Object는 { }안에 0개 이상의 프로퍼티가 있는 것. 즉, 프로퍼티의 집합
  
  ~~~javascript
  var book = {
      title: "책",
      point : 123
  }
  // 프로퍼티 key or name : 프로퍼티 value
  ~~~


<br>


## typeof 연산자
---------------------
- 데이터 타입 반환
~~~javascript
var point = 123;
console.log(typeof point);
// Output : number

var book = "책";
console.log(typeof book);
// Output : string
~~~
- typeof 연산자의 한계 : 설계 미스!
~~~javascript
// typeof로 null 과 Object를 구분할 수 없다.
console.log(typeof undefined);
// Output : undefined
console.log(typeof null);
// Output : null
~~~





  