# CSS3 기본학습

--------------------

## CSS3 기초 선택자와 단위
```
* { color : red }	//전체
h1 { color : red }	//태그
#header { color : red }	//id
.select { color : red }	//class
input[type="text"] { color : red } //속성
#header h1 { color : red }	//자손
#header > h1 { color : red }//후손
```

## CSS3 속성
```
#box{
            //박스 속성
            width: 50px;
            height: 50px;
            border: 5px;
            margin: 0;
            padding: 0;
            
            //가시 속성
            display: none;  //block, inline, inline-block
            
            //배경 속성
            background: black;
            
            //글자 속성
            font-size: 10px;
            font-family: Arial;
            
            //위치 속성
            position: absolute;
            
            //유동 속성
            float: left;
            
            //그림자 속성
            text-shadow: 5px 5px 5px black;
            box-shadow: 5px 5px 5px black;
    }
```

## 다양한 레이아웃의 구성과 기능
```
// 수평 정렬 레이아웃
div.container{
  overflow: hidden;
}
div.item{
  float:left;
}

//중앙 정렬 레이아웃
* {margin:0; padding:0;
body{ 
  margin: 0 auto;
  width: 960px;
}
```
* One True 정렬 레이아웃
[코드](https://github.com/choiyeonseong/StudyHtml/blob/main/02_CSS/layout_onetrue_test.html)

* 절대위치, 중앙 배치, 고정위치 배치
* 글자생략
```
.ellipsis{
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

## 반응형 웹
* 반응형 웹(Responsive Web)<br>:하나의 웹페이지로 여러 디스플레이에 자동으로 반응해서 변경되는 것
* 뷰포트 설정
```
<meta name='viewport' content='user-scalable=no, initial-scale=1'>
```
* 미디어 쿼리 설정
```
 @media (max-width: 499px) {
            body {
                background-color: red;
            }
        }
```
[연습 코드](https://github.com/choiyeonseong/StudyHtml/blob/main/02_CSS/responsive_test.html)

[이전](https://github.com/choiyeonseong/StudyHtml)
