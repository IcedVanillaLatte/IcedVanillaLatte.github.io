---
title: "(1) GitHub Page로 블로그 만들기"
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake]
toc: true
toc_sticky: true
published: true
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
---

GitHub Page로 블로그를 만들어보자. GitHub Page에서 자체 제공하는 테마도 있지만, 여기에서는 Jekyll 테마를 사용한다. 그 중에서도 가장 잘 팔리고 있는 Minimal Mistake 테마를 기준으로 작성했다.

---


## 1. 새 저장소 만들기(repository)

깃허브 페이지가 될 새 저장소를 만든다. 이때, *Repository name*을 `username.github.io` 으로 짓는다.

![새 저장소](https://files.slack.com/files-pri/T25783BPY-F8YCAF664/screenshot_2018-01-26_16.02.44.png?pub_secret=615fd6f28e){: width="50%"}

### GitHub Desktop 클라이언트

GitHhub Desktop 클라이언트를 설치하면, 로컬에서 좀 더 편하게 작업할 수 있다. GitHhub에서 만든 repository를 clone하여 내 컴퓨터로 가져오자.

![clone a repository](https://github.com/IcedVanillaLatte/chiching/blob/master/assets/github%20repository.JPG?raw=true){: width="50%"}

<!--깃허프 페이지는 *master branch* 에서 작업한 결과물이 posting 되는것 같다. -->


로컬에서 repository에 있는 파일을 생성, 수정, 삭제 등 작업을 수행했다면, GitHub 클라이언트에서 변경된 사항을 `commit`하고, `push` 하여 최종 결과물을 저장 및 동기화한다. 반대로 브라우저에서 작업을 수행한 경우 해당 변경사항들을 `pull`하여 내 로컬의 repository와 동기화시키자.

수정 작업의 경우, `summary (required)`에 간단한 변경 내역을 작성해야 `commit` 버튼이 활성화된다.

![image](https://user-images.githubusercontent.com/61964210/76523031-0720d980-64ab-11ea-9ded-a32462b65e11.png){: width="50"}




## 2. Jekyll 테마 적용하기

이용 가능한 Jekyll 테마를 고르자.
[https://jekyllthemes.io/](https://jekyllthemes.io/)

여기에서는 **minimal-mistakes** 테마를 고른다. 'Most stars' jekyll-theme 이기도 하다.

- 참고 사이트
	- [minimal-mistakes quick start guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
	- [minimal-mistakes github](https://github.com/mmistakes/minimal-mistakes)

Jekyll 테마를 설치하는 데에는 세 가지 방법이 있다.

> There are three ways to install: as a [gem-based theme](https://jekyllrb.com/docs/themes/#understanding-gem-based-themes), as a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/) (GitHub Pages compatible), or forking/directly copying all of the theme files into your project.

하지만, 나는 `gem` 도 `ruby`도 모르고, 이를 [설치](https://jekyllrb.com/docs/installation/windows/)하고 사용하려면 [윈도우10에 리눅스 환경](https://docs.microsoft.com/ko-kr/windows/wsl/install-win10?redirectedfrom=MSDN)도 만들어야 한다.
이러다 배보다 배꼽이 커져 시작도 하기 전에 지칠 수 있으므로, 그냥 통째로 가져오자.

![fork](https://mmistakes.github.io/minimal-mistakes/assets/images/mm-theme-fork-repo.png){: width="50%"}


GitHub Pages에서 제공하는 테마는 [여기서]((https://pages.github.com/themes/)) 볼 수 있다.


## 3. `_config.yml` 편집하기

본 테마의 설정 파일인 `_config.yml` 파일을 수정하자.

- 참고 사이트
	- [https://mmistakes.github.io/minimal-mistakes/docs/configuration/](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)

테마, 스킨, 사이트 이름 등을 편집할 수 있다.

테마는 gem-based method로 설치한 것이 아니므로, `remote-theme`을 선택하자.

``` yml
# theme : "minimal-mistakes-jekyll"
remote_theme : "mmistakes/minimal-mistakes"
minimal_mistakes_skin : "contrast"
```

  `theme`을 선택하면, 다음과 같은 Page build warning 메일을 받아볼 수 있다.

> You are attempting to use a Jekyll theme, "minimal-mistakes-jekyll", which is not supported by GitHub Pages. Please visit https://pages.github.com/themes/ for a list of supported themes.

``` yml
# theme : "minimal-mistakes-jekyll"
remote_theme : "mmistakes/minimal-mistakes"
minimal_mistakes_skin : "contrast"
```
disqus를 이용하여 댓글 기능을 넣을 수도 있다.

- 참고 사이트
	- <https://inasie.github.io/it%EC%9D%BC%EB%B0%98/2/>
	- <https://disqus.com/>


## 4. 상단 메뉴바 설정

- 참고 사이트
	- [https://mmistakes.github.io/minimal-mistakes/docs/navigation/](https://mmistakes.github.io/minimal-mistakes/docs/navigation/)

상단 메뉴바(Masthead) 설정을 위해, `_data/navigation.yml` 파일을 편집한다.


``` yml
main:
	- title: "Categories"
	  url: /categories/
	- title: "Tags"
	  url: /tags/
	- title: "External Link"
	  url: https://google.com
	  description: "Google"
```

브라우저 크기가 줄어들면 아래와 같이 상단 메뉴를 숨겨준다.

![image](https://mmistakes.github.io/minimal-mistakes/assets/images/mm-priority-plus-masthead.gif)


## 5. 작성자 소개

포스트 글 작성자를 소개하고 싶다면, `_data/authors.yml` 파일을 만들어 아래와 같이 key 별로 값을 입력하자.

``` yml
# /_data/authors.yml

Billy Rick:
  name        : "Billy Rick"
  bio         : "What do you want, jewels? I am a very extravagant man."
  avatar      : "/assets/images/bio-photo-2.jpg"
  links:
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      url: "mailto:billyrick@rick.com"
    - label: "Website"
      icon: "fas fa-fw fa-link"
      url: "https://thewhip.com"
    - label: "Twitter"
      icon: "fab fa-fw fa-twitter-square"
      url: "https://twitter.com/extravagantman"
```

`authors.yml`에 작성자 정보를 입력하고 나면, 포스트 글 작성시 YAML Front Matter에 아래와 같이 이름 값을 적어주거나, 은 정보만 추가해주면 된다.

``` yml
author: Billy Rick
```
프로파일을 활성화하면 된다.
``` yml
author_profile: true
```

포스트 글을 클릭하면 좌측 사이드 바에서 작성자 정보를 볼 수 있다.

## (필요시) private 저장소 만들기

private 저장소를 만들면, 작성한 글을 private 저장소에 임시 저장하여 두고, 필요할 때 public 페이지로 옮겨와 post할 수 있다.

`settings` > `Manage access`

![image](https://user-images.githubusercontent.com/61964210/76523322-9201d400-64ab-11ea-896e-7e0282707a89.png){:width="50%"}

private repository에 저장된 이미지도 링크를 가져와 GitHub page(public repository)에서 사용할 수 있다.


## 6. GitHub Page 대문 글 및 이미지

GitHub Page에 처음 접속했을 때 보이는 글이나 이미지는 `index.html`을 통해 편집할 수 있다.

![image](https://user-images.githubusercontent.com/61964210/79518325-c3ae2200-808b-11ea-8045-3b00a18c8de3.png)

``` yml
---
layout: home
author_profile: false
title: "Odds and ends"
excerpt: "Vanity of vanities"
header:
  overlay_image: /assets/images/IMG_2842.jpg
  caption: "Last modified on March 2020"
---
```

이 파일 편집을 통해 작성자를 소개할지 여부를 정하거나, 제목이나 소개 글, 이미지를 바꿀 수 있다.




<!--stackedit_data:
eyJoaXN0b3J5IjpbOTI0MTkyNDk0LDE1MjQ4NTE5MjksLTk0Nz
gyOTQ1M119
-->