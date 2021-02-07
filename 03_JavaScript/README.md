# Java Script

-----------------------------

## 자바스크립트 기본 문법
자바스크립트 기본 용어와 출력 방법
자료형과 변수
조건문과 반복문
익명, 선언적 함수

## 문서 객체 모델
DOM(Document Object Model) : 웹 브라우저가 HTML 파일을 분석하고 출력하는 방식
object ==  tag
문서 객체 선택
```
window.onload = function () { // 페이지 로드되었을 때 처리하는 이벤트
            var header = document.getElementById("header");
            console.log(header.innerText);

```
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_5.html)

문서 객체 조작
```
  window.onload = function () {
            // h1 태그의 배경 색상을 변경합니다.
            document.querySelector('h1').style.backgroundColor = 'red';

            // h2 태그의 글자 색상을 변경합니다.
            document.querySelector('h2').style.color = 'red';
        }
```
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_4.html)

이벤트
```
  window.onload = function () {
            // id 객체 가져오기
            var clock = document.getElementById("clock");
            // clock 객체의 html에 현재보다 3초전 시간 넣기
            setInterval(function () {
                var now = new Date();
                clock.innerHTML = now.toString();
            }, 3000);
        };
```
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_6.html)

## jQuery 라이브러리


## 자바스크립트와 jQuery 라이브러리 응용

[이전](https://github.com/choiyeonseong/StudyHtml)
