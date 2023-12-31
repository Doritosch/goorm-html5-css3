## HTML?
* Hyper Text Markup Language 의 약자
<br/>

### Hyper Text
* **하이퍼링크**를 이용해 독자가 원하는 순서에 따라 기존문서에서 다른문서로 넘어갈 수 있는 텍스트
### Markup Language
* 태그를 이용하여 문서나 데이터의 구조를 명시하는 언어

## CSS?
웹페이지의 스타일. 디자인을 정의하여 정리한 문서 <br>

### Cascading
* 우선순위에 따라 높은 것에서 낮은 것으로 화면에 적용하는 것
### Style Sheets
* 스타일 . 웹페이지의 색이나 글자 크기 및 폰트, 웹페이지의 구성요소 배치
<br/>
<br/>
<br/>

# HTML
컨텐츠 구조를 정의하는 마크업언어
컨텐츠에 태그를 씌워 구조를 구분하여 정의
<br/>
<br/>

<p align="center">
  <img src="https://wikimedia.org/api/rest_v1/media/math/render/svg/9b19f2818482c6618c82e23b4e6a5a3a4d94c57d" alt="html 요소">
<br>
html 요소
</p>
<br>

`<!DOCTYPE html>`
-----
문서의 가장 처음에 배치되어 이 문서가 html문서라고 브라우저에게 알려주는 역할

`<html lang = "ko">`
-----
* `<html>` 태그는 전체 HTML문서를 감싸는 태그
* HTML문서에서 단 한번 사용가능
* `<html>` 태그 바깥에는 다른 태그 존재 X
* lang = "ko"는 이 페이지의 주언어가 한국어라는 것
<br>
<br>

## Head와 Body
`<html>` 태그 안에는 크게 `<head>` 태그와 `<body>` 태그 존재

### Head
* HTML 문서에 대한 정보를 담고 있음
* 일반 사용자는 웹사이트에서 `<head>` 태그에 속한 내용을 볼 수 없음
* HTML문서 안에 단 하나 존재
* `<html>` 태그 바로 아래에 위치
  * `<meta>` : 문서와 관련된 정보를 담는 태그
   * `<title>` : 웹페이지의 제목을 담는 태그

### Body
* HTML 문서에서 사용자에게 실제로 보여지는 부분
* 문서내 단 하나 존재
* `<head>` 바로 아래에 위치
#### 제목 태그
  * `<h1>` : 제목을 표시하는 태그 <span style="color:#808080"> +중요도에따라 1~6까지 사용</span>
#### 본문 태그
  * `<p>` : 단락 혹은 문단
  * `<br>` : 줄바꿈
  * `<pre>` : 형식화된 텍스트를 브라우저에 그대로 표시
#### 나누기 위한 태그
  * `<div>` : 각각의 태그를 구분 짓기 위해 사용되는 태그, CSS를 이용하여 레이아웃을 배치할 때 CSS를 효과적으로 적용하기 위해서 사용
#### 글자와 관련된 태그
  * `<strong>` : 볼드체
  * `<em>` : 이탤릭체
  * `<sup>` : 태그로 감싼 단어 혹은 문장을 일반 위치보다 위로 올림
  * `<sub>` : 태그로 감싼 단어 혹은 문장을 일반 위치보다 아래로 내림
  * `<ins>` : 밑줄선
  * `<del>` : 취소선
#### 링크 태그
  * `<a>` : 하이퍼링크의 역할을 수행
    * href(Hypertext Reference) : `<a>` 가 참조하는 웹사이트 주소(경로)를 값으로 가지는 속성
    * target : 링크를 클릭했을 때 해당 페이지를 어디에서 열지 정하는 속성
      * _self : 현재 탭에서 링크 열기
      * _blank : 새 탭 혹은 새 창에서 링크 열기
  * **URL(Uniform Resource Locator)** : 주소(Address) + 경로(Path)
    * 절대 URL(Absolution URL) : 최초 시작점(주소)부터 경유한 경로를 모두 기록하여 리소스의 위치를 나타낸다.
    * 상대 URL(Relative URL) : 현재 위치(기준점)를 기준으로 상대적인 경로를 기록하여 리소스의 위치를 나타낸다.
<br>
<br>

## 기본적인 레이아웃
### Semantic tag
레이아웃을 태그로 만들어 각 요소의 쓰임을 명확하게 구분하는 것

* `<header>` : section의 소개나 제목
* `<nav>` : 페이지 이동을 위한 메뉴
* `<setion>` : 기준에 따라 구획을 구분하기 위해 사용하며, 기준에 맞는 `<article>` 들을 담는다
* `<article>` : 주내용을 담기위해 사용
* `<aside>` : 괄호 or 주변 부분에 해당하는 내용
* `<footer>` : 일반적으로 웹사이트의 가장 아래에 들어가는 추가 정보를 담기위해 사용하는 요소