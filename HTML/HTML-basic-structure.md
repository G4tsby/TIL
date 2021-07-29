# HTML 기본 구조

```HTML
<!DOCYTYPE HTML>
<html>
    <head>
        <title>HTML 기본 구조</title>
        <meta charset="UTF-8">
    </head>
    <body>
        HTML 5 기본 구조.
    </body>
</html>
```

<br>

```<!DOCTYPE HTML>``` : HTML5를 사용할 것임을 브라우저에 선언한다.  
```<html>``` : 전체 html을 감싸는 태그이다. `<html>` 태그 바깥에는 DOCTYPE 외에 다른 태그가 존재해서는 안된다.  
`<head>` : html 문서에 대한 정보나 설정 등을 담는다. `<html>` 태그 안에 존재해야 한다.  
`<title>` : 페이지의 제목을 담는 태그이다.  
`<meta>` : 문서에 대한 설명을 표시한다. `charset="UTF-8"` 은 문자 인코딩을 변경하는 지시이다.  
`<body> `: 실제적으로 화면에 보여지는 부분. `<html>` 태그 안에 존재해야 한다.  