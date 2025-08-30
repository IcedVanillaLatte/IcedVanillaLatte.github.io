---
title: "(6) Customizing"
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake, Mermaid Diagram, Disqus]
toc: true
toc_sticky: true
published: true
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
---

## Font size

Minimal Mistakes Theme으로 만든 페이지는 페이지에 접속하는 기기에 따라, 서로 다른 폰트 크기가 출력된다. 일반 모니터는 크게, 패드는 좀 작게, 스마트폰과 같은 작은 기기는 더 작은 폰트로 화면 크기에 맞게 폰트 사이즈가 자동을 조절된다.
이와 같이 **화면 크기에 따라 적용되는 폰트 사이즈**는 `_sass/minimal-mistakes/_reset.scss` 에서 조절 가능하다.
``` scss
	@include breakpoint($medium) {
	font-size: 18px;
	}
	@include breakpoint($large) {
	font-size: 20px;
	}
	@include breakpoint($x-large) {
	font-size: 22px;
	}
```

Default 값은 각각 18, 20, 22px 이다. 한글은 영어보다 폰트가 좀 더 크게 보이는 듯 하여, 적당히 사이즈 조절을 하는 편이 좋다.

- 참고 사이트
	- <https://devinlife.com/howto%20github%20pages/github-pages-settings/>

## Hyperlink colors

기본적으로 default 스타일은 `_sass` 디렉토리에 담겨있다. 이 스타일들을 변경하고 싶다면, `/assets/css/main.scss` 파일을 수정하여 나만의 스타일을 만들 수 있다.

**하이퍼링크 색깔**과 같은 폰트들에 대한 변수는 `_sass/minimal-mistakes/_variables.scss`에서 확인할 수 있다. 링크 색깔, 마우스 오버 했을 때의 링크 색깔, 방문한 링크의 색깔은 아래와 같다.

![image](https://user-images.githubusercontent.com/61964210/78757515-955b8300-79b7-11ea-82bc-2f72d7e162cc.png)

이 변수와 값들을 참조하여 `<your_project>/assets/css/main.scss`를 편집하여 `@import` 라인 앞에 다음과 같이 원하는 색깔을 추가하자. 

``` scss
$link-color: red; // or
$link-color: #338AFF;
```

- 참고 사이트
	- <https://mmistakes.github.io/minimal-mistakes/docs/stylesheets/>


## Hyperlink underline

**하이퍼링크의 밑줄**을 없애고 싶다면 아래 링크를 참고하자.

- 참고 사이트
	- [devinlife github page](https://github.com/devinlife/devinlife.github.io/commit/5440cf5eaf6ebd15b70754c778d8cab19a1203c3)


## Share link

Minimal Mistakes Theme 에서는 기본적으로 twitter, facebook, LinkedIn 으로의 공유 기능을 제공해준다. 이와 같은 SNS 공유 링크를 불러오는 파일은 `_includes/social-share.html`으로, 아래와 같이 작성되어 있다.
``` html
<a href="https://twitter.com/intent/tweet? (중략) </a>
<a href="https://www.facebook.com/sharer/sharer.php? (중략) </a>
<a href="https://www.linkedin.com/shareArticle? (중략) </a>
```
여기에 **카카오톡으로 공유**할 수 있는 버튼을 추가해보자.

먼저, [Kakao Developer](https://developers.kakao.com/)에 접속해서 "내 애플리케이션"을 만들고, 애플리케이션 설정에서 내 홈페이지를 플랫폼으로 추가한다.
![image](https://user-images.githubusercontent.com/61964210/78332140-6366ad00-75c2-11ea-8e99-aad2e1c400f2.png)

이후, "앱 키"에서 발급되는 javascript 키를 확인하고 메모장 등에 옮겨놓자.

그리고 카카오톡의 javascript를 사용할 수 있도록, `_includes/head.html` 파일의 `link` 태그 밑에 아래와 같이 카카오톡에서 받은 API key를 스크립트 안에 넣어주자.

``` html
<!-- For all browsers -->
<link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">

<!-- Kakao API -->
<script src="https://developers.kakao.com/sdk/js/kakao.min.js"></script>
<script type='text/javascript'>
Kakao.init('YOUR API KEY');
</script>
```

이제, twitter, facebook, LinkedIn 과 같이 `_includes/social-share.html`의 `section` 태그 안에 다음을 추가한다.
``` html
  <a id="kakao-link-btn" href="javascript:;"><img src="//developers.kakao.com/assets/img/about/logos/kakaolink/kakaolink_btn_small.png"/></a>
```
그리고 `section` 태그 밑에 `script` 태그를 새로 만들어 다음 내용을 추가한다.

``` html
</section>
<script type='text/javascript'>
    Kakao.Link.createDefaultButton({
      container: '#kakao-link-btn',
      objectType: 'feed',
      content: {title: "{{ page.title }}", imageUrl: '',link: {
          mobileWebUrl: '{{ page.url | absolute_url | url_encode }}',
          webUrl: '{{ page.url | absolute_url | url_encode }}'}
      },
      buttons: [{title: '웹으로 보기',link: {
            mobileWebUrl: '{{ page.url | absolute_url | url_encode }}',
            webUrl: '{{ page.url | absolute_url | url_encode }}'}},]
    });
</script>
```
- 참고 사이트
	- [카카오톡 API 사용해보기](https://imreplay.com/study/%EC%B9%B4%EC%B9%B4%EC%98%A4-API-%EC%82%AC%EC%9A%A9%ED%95%B4%EB%B3%B4%EA%B8%B0/)


## Comments

댓글을 남길 수 있는 **댓글 기능**을 사용해보자. [Disqus](https://disqus.com/)  에서 제공하는 댓글 서비스는 제한된 기능만 사용하여 무료로 가입하여 이용 가능하다. 가입하면 "short name"을 얻게 되는데, 이를 `_config.yml`에 적어주면 된다.

먼저 [Disqus](https://disqus.com/)에 가입하고, "Setting"에 들어가자.

![image](https://user-images.githubusercontent.com/61964210/78760557-4fed8480-79bc-11ea-8d13-154082c4d2ef.png)

"Add Disqus To Site"를 클릭해서 내 사이트를 등록하자.

![image](https://user-images.githubusercontent.com/61964210/78760628-672c7200-79bc-11ea-91ba-166220d2445b.png)

![image](https://user-images.githubusercontent.com/61964210/78760764-93e08980-79bc-11ea-84d1-2b46418d5247.png)

내 사이트를 등록하고 나면, 아래와 같이 사이트별 통계나 분석 정보를 볼 수 있는 메뉴가 생긴다.

![](https://downloads.intercomcdn.com/i/o/52810522/2a1d76b4f399da53e043eb74/dashboard-forums.png)

여기서 다시 "Setting" 메뉴에 들어가면, "General" 메뉴에서 shortname을 확인할 수 있다.

![image](https://user-images.githubusercontent.com/61964210/78761790-043bda80-79be-11ea-9c73-8b2a54c8902e.png)


이제, 여기서 얻은 shortname을 `_config.yml`에 적어주기만 하면 된다.

``` yml
comments:
  provider: "disqus"
  disqus:
    shortname: "your-disqus-shortname"
```

- 참고 사이트
	- <https://mmistakes.github.io/minimal-mistakes/docs/configuration/>
	- <https://help.disqus.com/en/articles/1717111-what-s-a-shortname>


## Diagram

[StackEdit](https://stackedit.io/app#) 에서는 다음과 같은 구문으로 code를 작성하면 **mermaid 다이어그램**을 출력할 수 있다.

```
	``` mermaid
	sequenceDiagram
		Alice ->> Bob: Hello Bob, how are you?
		Bob-->>John: How about you John?
		Bob--x Alice: I am good thanks!
		Bob-x John: I am good thanks!
		Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

		Bob-->Alice: Checking with John...
		Alice->John: Yes... John, how are you?
	```
```

![diagam in StackEdit](https://user-images.githubusercontent.com/61964210/76493619-5ef11d80-6476-11ea-8f05-7ee164699458.png)

하지만, GitHub Page에서 위와 같은 diagram을 출력하기 위해서는 추가 작업이 필요하다.


다이어그램 출력을 위해서는 jekyll 테마에 mermaid 플러그 인을 설치해야 하지만, 썩 매끄럽지 않은듯 하다.

> And jekyll has a [plugin](https://github.com/jasonbellamy/jekyll-mermaid) to simplify the creation of mermaid diagrams and flowcharts in your posts and pages. However, for safety reasons, if you want github automatically transform your post into web pages, you can’t use a plugin. So here I’ll show you how to make mermaid work in jekyll without plugin. \[[바로가기](http://kkpattern.github.io/2015/05/15/Embed-Chart-in-Jekyll.html)\]

대신, `mermaid` 스크립트를 `_includes/head.html`에 추가함으로써 웹에서도 다이어그램을 출력할 수 있다.

``` html
<script src="https://unpkg.com/mermaid@8.4.8/dist/mermaid.min.js"></script>
```

그리고 본문에서는 `div` 태그를 사용해 mermaid 형식의 글임을 나타내줘야 한다.

```
<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
</div>
```
> Next, we will change the jekyll template to include the mermaid code. In the `_includes` directory there is a file named `head.html`. Content in this file will be include in the head section of every page rendered by jekyll. And the chart definition need to be in a `div` whose class is `mermaid`.

하지만, 어차피 본문 글을 작성할 때, `<div class="mermaid">...</div>` 태그를 달거라면, 아래와 같이 `<script>...</script>` 태그도 본문에서 처리하는 편이 더 나을 수 있다.


``` html
<script src="https://unpkg.com/mermaid@8.4.8/dist/mermaid.min.js"></script>
<div class="mermaid">
graph TD
    A-->B
    A-->C
    B-->D
    C-->D
</div>
```
이 스크립트 구문은 아래와 같이 mermaid diagram으로 변환되어 표현된다.

<script src="https://unpkg.com/mermaid@8.4.8/dist/mermaid.min.js"></script>
<div class="mermaid">
graph TD
	A-->B
	A-->C
	B-->D
	C-->D
</div>

20년 4월 사용 가능한 `mermaid` 최신 버전은 `8.5.0`이며, 사용 가능한 스크립트 및 버전은 [여기에서](https://unpkg.com/mermaid/ "Index of the mermaid package") 확인할 수 있다.


- 참고사이트
	- <http://edgriebel.com/2019-embedding-mermaid-diagram/>
	- [Live Editor](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVERcbiAgQVtDaHJpc3RtYXNdIC0tPnxHZXQgbW9uZXl8IEIoR28gc2hvcHBpbmcpXG4gIEIgLS0-IEN7TGV0IG1lIHRoaW5rfVxuICBDIC0tPnxPbmV8IERbTGFwdG9wXVxuICBDIC0tPnxUd298IEVbaVBob25lXVxuICBDIC0tPnxUaHJlZXwgRltmYTpmYS1jYXIgQ2FyXVxuXHRcdCIsIm1lcm1haWQiOnsidGhlbWUiOiJkZWZhdWx0In19)







<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwODAyODk3MzgsLTEwOTcxMDI2OTIsMT
Q4NTQwMTI5LDExMDUxNDAyMF19
-->