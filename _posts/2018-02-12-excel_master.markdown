---
layout: post
title: 엑셀 10분만에 마스터하기
img: excel.png
---

<blockquote>
필자는 엑셀 도구를 참으로 좋아 합니다.
이처럼 훌륭한 계산기를 사용할 수 있다는 것은 더욱 기분 좋은 일이 아닐 수 없습니다.
특히, 정형 자동화 보고서와 비정형 맞춤 보고서를 작성할 때 엑셀을 활용하면, 물리적인 총량의 리소스 투입비용을 줄일 수 있는 성과를 얻을 수 있습니다.
스마트한 업무가 가능해 집니다.
직장 업무, 컨설팅, 강의 등을 하면서 수백만 로우데이터를 가공하여 분석 데이터를 산출한 경험을 바탕으로 10분만에 엑셀을 마스터할 수 있는 TIP을 공개 합니다.
몇 가지 함수만 익히면 순식간에 원하는 형태로 자료화할 수 있는 함수는 아래와 같습니다.
</blockquote>

{% highlight html %}
■ 합계 관련 함수
▷ sum()
▷ sumif()
▷ sumifs()
▷ sumproduct()

■계수 관련 함수
▷ count()
▷ countif()
▷ countifs()

■평균, 순위 관련 함수
▷ average()
▷ rank()
▷ large(), small(), max(), min()

■값 찾는 함수
▷ vlookup()
▷ hlookup()
▷ index()
    - 구조 ; index(찾는 값의 범위, 행번호, 열번호)
    -예제 : index($b2:$c10,match($d1,$a2:$a10,0),match($e1,$b1:$c1,0)),0)

▷ match()
▷ indirect() : [수식] - [이름관리자] - [이름 정의]로 활용
▷ address()
    - 구조 : address(행번호, 열문자)
    - 예제 : indirect(address($A1,3)) --> A1과 C열에 있는 주소의 값 찾음

▷ find()
    - 구조 : if(iserror(find("찾는 단어",문장위치)),0,1)
    - 예제 : if(iserror(find("1",$A1)),0,1)

■조건 값 구하는 함수
▷ if()
▷ if(and())
▷ if(or())
▷ iferror()

■표 안에 자동 정렬 배열 수식
배열수식 : Ctrl + Shift + Enter
{=INDEX($B$1:$B$5,MATCH(ROW(1:1),COUNTIF($B$1:$B$5,">=" & $B$1:$B$4),0))}
{% endhighlight %}

|  컨텐츠명  |    내용 확인 |
|----------|------------:|
| 엑셀 다른 시트로 이동 | <a href="http://sjmw1030.blog.me/221206932694"> 내용확인 </a> |
| 엑셀 위/아래 필드 비교 후 선착 순 등수 | <a href="http://sjmw1030.blog.me/221229785108"> 내용확인 </a> |
{: .table .table-striped .table-hover}
