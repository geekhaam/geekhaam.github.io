---

layout: post

title: "JSP: Day01 - HTML Basic"

comment: true

categories: JSP HTML Basic

---



*JSP(Java Server Page)를 배우기 앞서 HTML의 기초적인 지식을 알아봅니다. JSP는 HTML내에 자바 코드를 삽입하여 웹 서버에서 동적으로 웹 페이지를 생성하여 웹 브라우저에 돌려주는 언어이기 때문에 HTML에 대한 기본적인 지식이 선행되어야 합니다.*



# HTML 기초



Hyper Text Markup Language의 약자로 웹페이지를 제작할 때 기본 구조를 만드는 언어입니다.



* 용어 정리

1. 태그: 명령어의 형태가 <>로 되어있는 것들.

2. 요소: 태그의 시작(<>)과 끝(</>)의 한쌍을 의미.

3. 마크업: 요소들을 이용하여 웹문서를 작성하는 것.

4. 속성: 태그의 요소에 지정하는 것들.

ex) `<a href="#"?`에서 `href`를 속성이라 함.

___



* HTML 기본 구조



```html

<!DOCTYPE html>

<html>

<head>



</head>

<body>

</body>

</html>

```



1. `<DOCTYPE html>`: 현재 문서는 HTML 표준 규칙을 따른다는 의미입니다. 다양한 브라우저에서 마크업에 대한 일관된 화면 표시가 될 수 있도록 해줍니다.

2. `<html>`요소: 모든 html문서는 항상 이 요소 안에 마크업해야합니다. 기본적으로 `<head>`와 `<body>`요소로 구성되어 있습니다.

3. `<head>`요소: 문서의 속성이나 설정을 지정합니다.

	- head에 적는 대표적 요소

		* `<meta>`: 문서의 설명, 키워드, 저자 등을 지정

		* `<title>`: 문서의 제목 지정

		* `<link>`: 일반적으로 외부 CSS파일 연결시 사용

		* `<script>`: 주로 자바스크립트를 선언시 사용

		* `<style>`: 문서 내에서 직접 스타일(CSS)을 정의

4. `<body>`요소: 실제로 사용자에 보여질 화면을 마크업합니다.

___



* 블록 요소

	- 블록 요소는 마크업시 자동으로 줄바꿈이 일어나는 요소를 말합니다.

	- 블록 요소 안에는 텍스트와 인라인 요소를 포함할 수 있습니다.

	- 대표적으로 `<h1>` ~ `<h6>`, `<p>` 등이 있습니다.



```html

<h1>블록 요소</h1>

<h2>블록 요소 성질</h2>

<p>앞뒤로 줄 바꿈이 생깁니다.</p>

```



![block-elements](https://github.com/geekhaam/geekhaam.github.io/blob/master/assets/images/block-elements.PNG?raw=true "블록 요소")



___



* 인라인 요소

	- 인라인 요소는 마크업시 줄바꿈이 일어나지 않는 요소를 말합니다.

	- 인라인 요소 안에는 텍스트와 인라인 요소를 포함할 수 없습니다.

	- 인라인 요소는 블록 요소를 포함할 수 없습니다.

	- 인라인 요소는 블록 요소 안에 포함시키는 것이 좋습니디.



```html

<h1>인라인 요소</h1>

<h2>인라인 요소 성질</h2>

<p>

		<strong>인라인 요소는 한 줄로 출력됩니다.</strong>

	<a href="#">인라인 요소 링크</a>

</p>

```



![inline-elements](https://github.com/geekhaam/geekhaam.github.io/blob/master/assets/images/inline-elements.PNG?raw=true "인라인 요소")



