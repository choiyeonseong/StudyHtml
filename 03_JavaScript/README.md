# Java Script

-----------------------------

## 자바스크립트 기본 문법
* 자바스크립트 기본 용어와 출력 방법
* 자료형과 변수
* 조건문과 반복문
* 익명, 선언적 함수

## 문서 객체 모델
* DOM(Document Object Model) : 웹 브라우저가 HTML 파일을 분석하고 출력하는 방식
object ==  tag
* 문서 객체 선택 <br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_5.html)
```
window.onload = function () { // 페이지 로드되었을 때 처리하는 이벤트
            var header = document.getElementById("header");
            console.log(header.innerText);

```

* 문서 객체 조작<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_4.html)
```
  window.onload = function () {
            // h1 태그의 배경 색상을 변경합니다.
            document.querySelector('h1').style.backgroundColor = 'red';

            // h2 태그의 글자 색상을 변경합니다.
            document.querySelector('h2').style.color = 'red';
        }
```

* 이벤트<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/js_test_6.html)
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

## jQuery 라이브러리

* jQuery 라이브러리 설정

* 문서 객체 선택<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_1.html)
```
 $(document).ready(function () {
            // alert("Hello World");
            $('h1').css('background-color', 'black');
            $('h1').css('color', 'white');
```
* 문서 객체 조작<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_1.html)
```
 $(document).ready(function () {
            console.log($('script').attr('src'));
```


* 이벤트<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_2.html)
```
 $(document).ready(function () {
             $('#box').css({
                width: 100,
                height: 100,
                background: 'orange'
            }).on('click', function () {
                $(this).css({
                    background: "red"
                });
            }).on("mouseenter", function () {
                $(this).css({
                    background: "blue",
                    borderRadius:"50%"
                });
            }).on("mouseleave", function () {
                $(this).css({
                    background: "orange",
                    borderRadius:"0%"
                });
            });
        });
```

* 시각 효과<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_3.html)
```
$(document).ready(function () {
            $('#box').css({
                width: 100,
                height: 100,
                background: 'red'
            }).animate({
                width: 400,
                opacity: 0.5,
            }, 1000); // 1000ms = 1초
        });
```

## 자바스크립트와 jQuery 라이브러리 응용
* 입력 양식 포커스<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_4.html)
* 프레임 애니메이션
* 문서 객체 생성과 추가<br>
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_test_5.html)
* 무한 스크롤 
* 플러그인 사용 <br>
[lightbox](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_lightbox_text.html)<br>
[masonry](https://github.com/choiyeonseong/StudyHtml/blob/main/03_JavaScript/jquery_gridlayout_test.html)
* 갤러리

[이전](https://github.com/choiyeonseong/StudyHtml)
