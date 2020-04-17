---
title: "GitHub Page: (3) Posting"
categories: IT
tags:
  - GitHub Page
  - Minimal Mistake
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

## 2. YAML Front Matter

모든 블로그의 포스트 파일은 반드시 [YAML front matter](https://jekyllrb.com/docs/front-matter/)로 시작해야 한다. YAML front matter는 포스트 글의 메타 데이터를 담고 있다.

``` yml 
---
title: "Welcome"
date: 2020-03-10 12:39:00 +0900
categories: Github Pages
---
```
YAML Front matter의 `title`에 작성한 글이 해당 포스트의 제목으로 표시된다.

테마에 따라서 여기에 들어가는 정보가 조금씩 다를 수 있으므로, 각 테마별로 YAML front matter 규칙을 살펴볼 필요가 있다.


## 3. Publish

publish 할 때, 제목의 띄어쓰기는 상관이 없다. .다만, 경로(_posts/filename)만 주의하자.
파일 제목은 repository에 올라가는 파일 이름일 뿐, YAML Front Matter의 `title`에 작성된 문구가 해당 포스트의 제목이 된다. YAML Front Matter 상에 다음과 같은 구문으로 publish 여부를 선택할 수도 있다.

``` yml 
---
title: "Welcome"
date: 2020-03-10 12:39:00 +0900
categories: Github Pages
p
# . ublished: true
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
title: "Welcome"
date: 2020-03-10 12:39:00 +0900
categories: Github Pages
toc: true
toc_label: "My Table of Contents"
toc_icon: "cog"
toc_sticky: true
published: true
---
```

## 6. Sidebar

만약 한 주제로 여러 글들을 연속해서 나누어 포스팅한다면, 관련된 글들을 모아 보여줌으로써 전체 글의 흐름을 파악할 수 있을 것이다. 이를 sidebar에 나타나도록 하려면, `_data/navigation.yml`을 편집하면 된다.

```




``` yml
sidebar:
  nav: "docs"
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNjk4NzMxNiwtMTA4MDczNDk4MCwtMT
gyODU3NTY3NSwyMDE1NTAyMjU5LC0xODQ1NDAyNDY3LDE0NTYz
ODUyOTAsLTIwOTM2Mzk1NTMsLTM5NzUzNTc0LC0xMzkzMzI2NT
JdfQ==
-->