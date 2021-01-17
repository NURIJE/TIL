# hello.js
<br>

## html에 js파일 삽입하는 방법
-------------------------
⬇️ `<head>` 부분에 작성
~~~html
<head>
    <script src="hello.js" defer></script>
</head>
~~~
⬇️ `<body>` 부분에 작성
~~~html
<body>
    <script src="hello.js" defer></script>
</body>
~~~
<br>

## defer 속성
-------------------------
- head 부분에 자바스크립트 파일를 삽입하면 서버에서 파일을 가져와 코드를 실행함. 
- 해당 코드에서 body에 있는 element에 접근하면 아직 body가 렌더링 되지 않았기 때문에 에러가 발생할 수 있음.
- defer 속성을 작성하면 body가 모두 랜더링된 후에 해당 자바스크립트 코드를 실행함.