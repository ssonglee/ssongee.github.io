---
layout: post
title:  "마크다운(Markdown) 문법 정리"
subtitle: "알아두면 피가 되고 살이되는 마크다운 문법정리 :)"
type: "Markdown"
etc: true
text: true
order: 1
date: 05 Mar 2019
---

<strong>1. 헤더(Header)</strong>

<br>
헤더 크기는 1~6까지 지원한다.<br>
```
# This is H1        
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6
```

# This is H1        
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6

<br><br>

<strong>2. 인용구</strong>

<br>
인용구는 ```>```를 이용한다. 인용구 안에서 다른 마크업 요소를 섞어서 사용할 수 있다.<br>
```
> 안녕
> > 안녕
> > * 안녕
> > > * 안녕
```
> 안녕
> > 안녕
> > * 안녕
> > > * 안녕

<br><br>

<strong>3. 목록</strong>

<br>
 - 순서가 있는 목록<br>

```
  1. 일번
  2. 이번
  3. 삼번
```
1. 일번
2. 이번
3. 삼번


- 순서가 없는 목록<br>

```
* 일번
  * 이번
    * 삼번
+ 일번
  + 이번
    + 삼번
- 일번
  - 이번
    - 삼번
```
* 일번
  * 이번
    * 삼번

+ 일번
  + 이번
    + 삼번

- 일번
  - 이번
    - 삼번

<br><br>

<strong>4. 코드</strong>

<br>
&lt; pre > &lt; code > 에 감싸서 사용한다.<br>

```
<code>Github</code>
```
<code>Github</code>
<br><br>

```
  <pre><code>
  for i in range(1,2):
    print(i)
  </code></pre>
```

<pre><code>for i in range(1,2):
  print(i)
</code></pre>

<br><br>
ps. 코드 하이라이터를 사용하는 경우(내 지킬 블로그 테마) js 대신에 원하는 언어를 넣을 수 있다. [Rouge](http://rouge.jneen.net/) 하이라이터가 적용 되었다. <br>

<img src="https://user-images.githubusercontent.com/20412850/34469050-b6bb5f2e-ef59-11e7-8057-037fcbee07cf.png" width="30%">

{% highlight python %}
for i in range(1,2):
  print(i)
{% endhighlight %}

<br><br>

<strong> 5. 수평선 </strong>

<br>

```
------
************
```

------
************

<br><br>

<strong> 6. 링크 </strong>

<br>
 - 인라인 링크

 ```
 [Google](http://google.com)
 ```
 [Google](http://google.com)

<br>
  - 자동 연결 링크

```
<http://google.com>
```
<http://google.com>

<br><br>

<strong>8. 강조</strong>

<br>
진하게, 기울기, 취소선이 있다. 밑줄은 지원하지 않는다.

```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```

*single asterisks*<br>
_single underscores_<br>
**double asterisks**<br>
__double underscores__<br>
~~cancelline~~<br>

<br><br>

<strong>9. 이미지</strong>

<br>

```
![이미지 이름](이미지 url)로 이미지를 넣을 수 있다.
![Image name](https://user-images.githubusercontent.com/20412850/34468412-ba059536-ef4b-11e7-90d4-3313e9fed8f9.png)
```
![Image name](https://user-images.githubusercontent.com/20412850/34468412-ba059536-ef4b-11e7-90d4-3313e9fed8f9.png)

<br><br>
  ps. 사이즈 조정

```
<img src="이미지 url" width="원하는 크기">
<img src="https://user-images.githubusercontent.com/20412850/34468412-ba059536-ef4b-11e7-90d4-3313e9fed8f9.png" width="60%">
```
<img src="https://user-images.githubusercontent.com/20412850/34468412-ba059536-ef4b-11e7-90d4-3313e9fed8f9.png" width="60%">


<br><br>

<strong>10. 표 그리기</strong>

<br>
표는 마크다운 표를 generate 해주는 사이트가 있다. 원하는 양식에 맞춰서 만들어서 갖다가 쓰면 편하다.

* 표 generate 사이트 : https://www.tablesgenerator.com/markdown_tables<br>

```
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell
```
<br>

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

내용 정렬은 아래와 같이 한다.<br>

```
First Header  | Second Header | Third Header
:------------ | :-----------: | -----------:
Left          | Center        | Right
```
<br>

First Header  | Second Header | Third Header
:------------ | :-----------: | -----------:
Left          | Center        | Right

<br><br>

<strong>11. 수식(테마에서 지원)</strong>

<br>
```
$$ f(x) = \int \frac{2x^2+4x+6}{x-2} $$
```
$$ f(x) = \int \frac{2x^2+4x+6}{x-2} $$

<br><br><br><br><br>