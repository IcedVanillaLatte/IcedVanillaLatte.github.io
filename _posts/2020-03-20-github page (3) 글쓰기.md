---
title: "(3) 게시글 포스팅하기"
date: 2020-03-16 09:00:00 +0900
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake]
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
toc: true
toc_sticky: true
published: true
---

- 참고 사이트
	- <https://jekyllrb.com/docs/posts/>
	- <https://mmistakes.github.io/minimal-mistakes/docs/posts/>


## 1. Create a file

블로그의 포스트는 자신의 GitHub 저장소의 `_post` 경로에 [Markdown](https://daringfireball.net/projects/markdown/)으로 작성된다. 그리고 파일 이름은 반드시 다음과 같은 형식을 지켜야 한다.
```
YEAR-MONTH-DAY-title.md
```
`YEAR`는 4자리, `MONTH`와 `DAY`는 2자리 숫자로 작성한다. `title`은 **띄어쓰기가 허용**된다.

날짜와 포스트의 제목 사이에 `-`를 빼먹지 않도록 유의하자.
{: .notice--warning}

까다롭고 귀찮은 형식이긴 한데, 아직 완성되지 않은 작성중인 게시글이 있다면 `YEAR-MONTH-DAY` 를 빼고 `title.md`로만 저장하는 방법으로 파일을 관리할 수 있다.

Jekyll 테마에서는 파일명에 적힌 `YEAR-MONTH-DAY`가 아래와 같이 게시글의 목록을 볼 때 제목 밑에 표시가 되며, 게시글이 정렬될 때도 이용된다. 

![image](https://user-images.githubusercontent.com/61964210/203225223-a15376ec-5743-47f7-b4a9-609069cebb97.png)



## 2. YAML Front Matter

모든 블로그의 포스트 파일은 반드시 [YAML front matter](https://jekyllrb.com/docs/front-matter/)로 시작해야 한다. YAML front matter는 포스트 글의 메타 데이터를 담고 있다.

``` yml 
---
title: "(3) 게시글 포스팅하기"
date: 2020-03-16 09:00:00 +0900
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake]
---
```
YAML Front matter의 `title`에 작성한 글이 해당 **포스트의 제목**으로 표시된다.

여기에서 작성되는 `date`는 md 파일명에 작성된 `YEAR-MONTH-DAY`를 overwrite 하는 효과가 있다. 혹 게시글 작성 후 수정을 하여 수정된 날짜로 올리고 싶다면, 파일명을 바꾸기 보다 YAML Front matter의 `date` 값을 바꾸는게 더 좋을 것 같다. YAML Front Matter에 `date`가 없다면, 파일 `YEAR-MONTH-DAY-title.md`에 작성된 연, 월, 일이 사용된다.

테마에 따라서 여기에 들어가는 정보가 조금씩 다를 수 있으므로, 각 테마별로 YAML front matter 규칙을 살펴볼 필요가 있다. `categories`와 `tag`는 `[]`안에 작성하여 표현할 수 있다.


## 3. Publish

publish 할 때, `title`의 띄어쓰기는 상관이 없다. 다만, 경로만 주의하자. 게시글이 `_posts/` 폴더 안에 있어야 한다.
파일 제목은 repository에 올라가는 파일 이름일 뿐, YAML Front Matter의 `title`에 작성된 문구가 해당 포스트의 제목이 된다. YAML Front Matter 상에 다음과 같은 구문으로 publish 여부를 선택할 수도 있다.

``` yml 
---
published: true
---
```

## 4. Markdown Editor

많은 블로그에서 Atom과 함께 Markdown preview enhanced 확장 프로그램을 추천한다. 하지만 나는 개인적으로 [StackEdit](https://stackedit.io/app#) 편집기가 제일 좋은 것 같다.
별도의 설치 없이 웹에서 사용 가능하고, 크롬 브라우저의 확장 프로그램으로도 사용할 수 있다. 또한 지원하는 마크다운 문법이 더 풍성하다. GitHub Page와의 동기화도 편하다. 자신의 구글 계정으로 접속하면, 에버노트처럼 카테고리를 구분해서 여러 글들을 작성하고 여러 장치에서 접근해서 보고 편집할 수 있다.

![image](https://user-images.githubusercontent.com/4952571/38148090-eb4ff8fa-348f-11e8-90e3-8b585a1c31ab.png)

StackEdit에서 작성한 글을 GitHub Page로 올리고 싶다면, 오른쪽 메뉴바에서 *Synchronize*를 선택하고, *Save on GitHub*를 누른다.

![image](https://user-images.githubusercontent.com/61964210/77400558-bbe1c180-6dee-11ea-803a-d670c3b8b9eb.png)

경로 지정시, 반드시 파일 이름 앞에 `_posts/`를 붙여주자. `_posts`폴더 안에 있는 파일이 GitHub Page에 포스트 글로 올라온다.


## 5. TOC

참고 사이트: <https://mmistakes.github.io/minimal-mistakes/docs/helpers/>

YAML Front Matter에 다음과 같이 toc 옵션을 추가하여 Table of Content를 포스트 글에 넣을 수 있다.

``` yml 
---
toc: true
toc_label: "My Table of Contents"
toc_icon: "cog"
toc_sticky: true
---
```

## 6. Sidebar

만약 한 주제로 여러 글들을 연속해서 나누어 포스팅한다면, 관련된 글들을 모아 보여줌으로써 전체 글의 흐름을 파악할 수 있을 것이다. 이를 sidebar에 나타나도록 하려면, `_data/navigation.yml`을 편집하면 된다.

``` yml
github:
  - title: "시작하기"
    url: /github%20page/github-page-(1)-시작하기
  - title: "레이아웃 정하기"
    url: /github%20page/github-page-(2)-레이아웃
  - title: "글쓰기"
    url: /github%20page/github-page-(3)-글쓰기
  - title: "LaTex 수식 표현하기"
    url: /github%20page/github-page-(4)-LateX-Expression
  - title: "이미지 올리기"
    url: /github%20page/github-page-(5)-Image-upload
  - title: "꾸미기"
    url: /github%20page/github-page-(6)-customizing
```

`title`은 navigation bar에 보여질 제목을 의미하며, `url`은 해당 제목을 클릭할 때 이동할 링크를 나타낸다. 게시글의 `url`은 작성된 게시글 파일의 `categories`와 `YEAR-MONTH-DAY-title.md` 파일의 `title`의 조합으로 정해진다.
- `categories`에 공백(띄워쓰기)이 있다면, `%20`으로 채워주자.
- `title`에 있는 공백은 `-`로 채워줘야 한다.

한땀 한땀 짜주다보면, 내가 왜 naver blog를 하지 않고 github page를 시작한 것인지 조금 후회가 될 수 있다.

**url 링크 작성시 유의사항:** 포스팅한 글들의 url은 해당 포스트의 **카테고리**에 따라 url이 만들어진다. 따라서, **카테고리**와 **타이틀**을 잘 구분해서 url을 작성해주자. 또한, 공백문자는 `-`으로 매꿔주자.
{:.notice--warning}

그리고 `_data/navigation.yml` 에서 사용한 키(여기서는 `github`)를 해당 글의 YAML Front Matter에 다음과 같이 추가해주자.

``` yml
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
```
`title` 및 `nav` 키를 `tab`으로 띄우지 말고, 공백 문자로 띄우자.
{:.notice--warning}

최종적으로, 본 게시글에 사용된 YAML Front Matter는 다음과 같다.
``` yml
title: "(3) 게시글 포스팅하기"
date: 2020-03-16 09:00:00 +0900
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake]
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
toc: true
toc_sticky: true
published: true
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2MzI1MzgwMzksLTIxMDI2MDU1NTksMT
AxNzk3Njk4MCwtMTk0NzUzNDc0OSw5MjIyMjg3MDcsMTg2NjQ1
MTEzOSwyMTAxOTY5NDIzLC0xMDgwNzM0OTgwLC0xODI4NTc1Nj
c1LDIwMTU1MDIyNTksLTE4NDU0MDI0NjcsMTQ1NjM4NTI5MCwt
MjA5MzYzOTU1MywtMzk3NTM1NzQsLTEzOTMzMjY1Ml19
-->