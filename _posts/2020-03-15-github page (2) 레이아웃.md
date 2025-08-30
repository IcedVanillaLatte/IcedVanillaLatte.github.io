---
title: "(2) Layouts 설정하기"
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake]
toc: true
toc_sticky: true
published: true
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
---

## Default layout

- 참고 페이지
	- <https://mmistakes.github.io/minimal-mistakes/docs/layouts/>

Layout을 변경하는 방법은 크게 두가지이다.
- `_config.yml`에서 default YAML front matter 값으로 일괄 설정하기
- 각각의 YAML front matter 값으로 개별 설정하기

`_config.yml`에서 설정 가능한 default YAML front matter 형식은 다음과 같다.

``` yml
# Front Matter Defaults
defaults:
	# _posts
	- scope:
		path: ""
		type: posts
	values:
		layout: single
		author_profile: false  # true (default)
		read_time: true
		comments: true
		share: true
		related: true
```

## Posts & Pages layout

일반적인 포스트 및 페이지에 적용 가능한 layout은 크게 **single** 과 **splash**로 구분된다. 먼저, 각 layout의 특징을 살펴보자.

Includes:|Single layout|Splash layout
---|:---:|:---:
Optional header image with caption| O | O
Optional header overlay (solid color/image) + text and optional “call to action” button|O|O
Optional social sharing links module|O|X
Optional comments module|O|X
Optional related posts module|O|X
Wide page variant|O|X
Feature blocks (`left`, `center`, and `right` alignment options)|X|**O**

|![image](https://user-images.githubusercontent.com/61964210/76681962-441bd600-663b-11ea-9831-472bdcc68c7b.png)|
|:---:|
|*`single` layout*|

|![image](https://mmistakes.github.io/minimal-mistakes/assets/images/mm-layout-splash.png)|
|:---:|
|*`splash`* layout|

Single layout은 일반적인 글을 포스팅할 때 좋은 것 같고, Splash layout은 여러 글이나 이미지 등을 함께 모아 보여주는 페이지를 만들 때 유용할 것 같다.


### (Sample) YAML Front Matter : Optional header image with caption

글을 포스팅할 때 해당 포스트를 대표할 만한 이미지가 있다면, 헤더에 관련 이미지를 삽입하는 방식이다.

``` yml
header:
  image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
```
위 표에서 보듯, Single layout과 Splash layout 모두 적용이 가능하다.

### (Sample) YAML Front Matter : Optional header overlay (solid color/image) + text and optional “call to action” button

삽입된 이미지 위에 글을 작성하거나 `action`버튼을 만들어 링크를 걸어주는 방식이다. 

``` yml
excerpt: "This post should display a **header with an overlay image**, if the theme supports it."
header:
  overlay_image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  actions:
    - label: "More Info"
      url: "https://unsplash.com"
```

`overlay_image`대신, `overlay_color`를 사용할 수도 있다.
``` yml
header:
  overlay_color: "#333"
```
마찬가지로, Single layout과 Splash layout 모두 적용이 가능하다.

### Single layout : Wide page variant

Single layout에 아래와 같은 옵션을 YAML Front Matter에 추가하여 적용할 수 있다. `wide` 옵션은 컨텐츠를 오른쪽으로 더 확장시킨다. TOC(Table of Contents) 가 설정되어 있는 경우, 기존 오른쪽 공간에 있던 TOC가 강제로 제목 밑에 위치하게 된다.

``` yml
classes: wide
```

Single layout에만 적용이 가능하다.

### Splash layout : Feature blocks

이미지나 비디오 등 여러 feature들을 정렬하거나 모아서 보여줄 수 있다. YAML Front Matter 및 샘플 페이지는 아래를 참고하자.
- 참고 사이트
	- [YAML Front Matter](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#feature-row)
	- [샘플 페이지(md)]([https://github.com/mmistakes/minimal-mistakes/edit/master/docs/_pages/splash-page.md](https://github.com/mmistakes/minimal-mistakes/edit/master/docs/_pages/splash-page.md))

Splash layout에만 적용이 가능하다.

## Tags layout

Tag 별로 포스트 글을 모아주는 Tag 페이지는 `layout: tags`를 사용하여 `_pages/`에 만들어 줄 수 있다.


`layout: tags`는 `layout: archive`와 같은 YAML Front Matter를 제공한다.

Includes:|Single layout|Archive layout
---|:---:|:---:
Optional header image with caption| O | O
Optional header overlay (solid color/image) + text and optional “call to action” button|O|O
Optional social sharing links module|O|X
Optional comments module|O|X
Optional related posts module|O|X
Wide page variant|O|X
List and grid views|X|**O**

작성된 글의 Tag를 모아서 **Tag별로 글을 정리해서 볼 수 있는 페이지**를 만들고 싶다면, 적당한 이름을 지어 아래와 같은 YAML Front Matter를 마크다운 `.md`파일로 만들어 `_pages` 안에 두자.

```yml
---
title: "Posts by Tag"
layout: tags
permalink: /tags/
author_profile: false  # true
---
```

상단 메뉴바의 **Tags** 를 클릭해 Tag 페이지에 접속할 수 있도록`_data/navigation.yml`에 아래와 같이 추가해주자.

```yml
main:
	- title: "Tags"
	  url: /tags/
```

작성된 페이지의 `permalink`의 경로와 메뉴를 클릭했을 때 이동할 `url` 경로가 같은지 확인하자.
{: .notice--warning}

## Categories layout

Category 별로 포스트 글을 모아주는 Category 페이지는  `layout: categories`를 사용하여 `_pages/`에 만들어 줄 수 있다. Category와 Tag가 어떤 차이가 있는지는 아직 잘 모르겠다.

마크다운 `.md` 파일의 YAML Front Matter는 다음과 같다.
```yml
---
title: "Posts by Category"
layout: categories
permalink: /categories/
author_profile: false  # true
---
```
`layout: tags`와 마찬가지로, `layout: categories`는 `layout: archive`와 같은 YAML Front Matter를 제공한다.

상단 메뉴바의 **Categories** 를 클릭해 Categories 페이지에 접속할 수 있도록`_data/navigation.yml`에 아래와 같이 추가해주자.

```yml
main:
	- title: "Categories"
      url: /categories/
```

작성된 페이지의 `permalink`의 경로와 메뉴를 클릭했을 때 이동할 `url` 경로가 같은지 확인하자.
{: .notice--warning}


### Table of Contents

목차(Table of Contents)를 표시해준다. toc를 활성화하는 경우, 선택 가능한 옵션은 아래와 같다.

```yml
--- 
toc: true
toc_sticky: true
toc_label: "My Table of Contents"
toc_icon: "cog"
---
```

사용 가능한 TOC 아이콘은 [여기에서](https://fontawesome.com/icons?d=gallery&s=solid&m=free) 확인할 수 있다.


------

그 밖의 Minimal Mistakes 에서 지원하는 다양한 레이아웃은 [참고 사이트](https://mmistakes.github.io/minimal-mistakes/docs/layouts/)를 통해 확인하자.

## Post date

Single layout 으로 글을 작성하면 포스트의 제일 밑에 Updated 날짜가 표시된다.![image](https://user-images.githubusercontent.com/1376749/42345790-806820aa-806e-11e8-8abe-5a2fe772e893.png)

하지만, 이를 제목 바로 아래에 두고 보고 싶을 수 있다. 

사실 YAML Front Matter의 `read_time: true` 옵션을 통해 보여지는 "글을 읽을 때 걸리는 시간"은... 개인적으로는 한 번도 궁금한 적이 없다.

- 참고사이트(폰트 사이즈 수정, 메뉴바 사이즈 수정, 포스트 제목 아래 게시 날짜 표시 등)
	- <https://devinlife.com/howto%20github%20pages/github-pages-settings/>

**포스트 글의 제목 바로 밑에 date를 추가**하고 싶다면, `_layout/single.html`을 [다음](https://github.com/IcedVanillaLatte/IcedVanillaLatte.github.io/commit/0359e29eb3ad1badf7a68b70d4f7e2da3ff820d5)과 같이 수정하여, `page__meta` 클래스 대신에 `page__date` 클래스로 바꾸자. 

**아카이브 페이지에서 `read_time` 대신 `date`를 표시**하고 싶다면, `_includes/archive-single.html`을 [다음](https://github.com/devinlife/devinlife.github.io/commit/c6a8fe5a2f2a6f208b4ad90528074842e5c3ee66)과 같이 수정하자. 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI5NjEzODA3NiwxOTY3MzY5NTM4LC0yMD
kyNjA1NTg5LC0zMDc2MDQyMDQsLTEwNzU3NjI4NDAsLTE2ODY2
ODE3MzAsLTkxMzE4NzIwMSwtMTc4NDMwMTE3MSwtOTI2ODYwNT
kxLC03MTc5NDE0NTJdfQ==
-->