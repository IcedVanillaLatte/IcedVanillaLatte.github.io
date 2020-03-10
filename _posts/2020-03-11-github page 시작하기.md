---
title: "깃허브 페이지 시작하기"
date: 2020-03-10 12:39:00 +0900
categories: Github Pages
toc: true
---

# 깃허브 페이지 시작하기


참고 사이트
1. <https://dreamgonfly.github.io/2018/01/27/jekyll-remote-theme.html>

[toc]


## 1. 새 저장소 만들기(repository)

깃허브 페이지가 될 새 저장소를 만든다. 이때, *Repository name*을 `username.github.io` 으로 짓는다.

![새 저장소](https://files.slack.com/files-pri/T25783BPY-F8YCAF664/screenshot_2018-01-26_16.02.44.png?pub_secret=615fd6f28e)

Github Desktop 클라이언트를 설치하면, 로컬에서 좀 더 편하게 작업할 수 있다. Github에서 만든 repository를 clone하여 내 컴퓨터로 가져오자.

![clone a repository](https://github.com/IcedVanillaLatte/chiching/blob/master/assets/github%20repository.JPG?raw=true){: width="50%"}


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

![fork](https://mmistakes.github.io/minimal-mistakes/assets/images/mm-theme-fork-repo.png)


GitHub Pages에서 제공하는 테마는 [여기서]((https://pages.github.com/themes/)) 볼 수 있다.


## 3. `_config.yml` 편집하기

본 테마의 설정 파일인 `_config.yml` 파일을 수정하자.

- 참고 사이트
	- [https://mmistakes.github.io/minimal-mistakes/docs/configuration/](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)

테마, 스킨, 사이트 위치, 이름 등을 편집할 수 있다.

테마는 gem-based method로 설치한 것이 아니므로, `remote-theme`을 선택하자.  `theme`을 선택하면, 다음과 같은 Page build warning 메일을 받아볼 수 있다.

> You are attempting to use a Jekyll theme, "minimal-mistakes-jekyll", which is not supported by GitHub Pages. Please visit https://pages.github.com/themes/ for a list of supported themes.

``` yml
# theme : "minimal-mistakes-jekyll"
remote_theme : "mmistakes/minimal-mistakes"
minimal_mistakes_skin : "contrast"
```

## 4. index 파일 가져오기
Jekyll이 사이트를 생성할 때 가장 처음 보여주는 페이지로, `index.html`을 가져온다.

## 5. 새 글 쓰기

- 자신의 GitHub 저장소에서 Create new file을 눌러 새 파일을 생성한다.
- 파일 이름에 `_posts/2018-01-26-first-post.md`을 입력한다.
- 이 때 `/` 앞의 `_posts`는 폴더 이름으로 인식되며 GitHub에서 자동으로 폴더를 생성한다. Jekyll은 `_posts` 아래의 markdown 글들을 블로그 포스트로 인식하고 블로그에서 보여준다. 파일 이름은 일반적으로 `YYYY-MM-DD-name-of-post.md` 형식으로 짓는다.
- 파일 내용 맨 처음에는 다음과 같이 글의 제목과 날짜 등을 적어줍니다. 이 형식은 **Front matter** 라고 불리며, Jekyll에서 글의 메타 데이터를 확인하는 방법이다.

``` markdown_ext
---
title: "깃허브 페이지 시작하기"
date: 2020-03-10 12:39:00 +0900
categories: Github Pages
toc: true
---
```


- 테마에 따라서 여기에 들어가는 정보가 조금씩 다를 수 있으니 각 테마 별로 예시 확인 필요

## 6. private 저장소 만들기

private 저장소를 만들면, 작성한 글을 private 저장소에 임시 저장하여 두고, 필요할 때 public 페이지로 옮겨와 post할 수 있다.

`settings` > `Manage access`

![private access](/assets/toc.png)

이미지도 여기에 두고 사용하면, 내가 올린 이미지가 공개적으로 사용되는 것을 막을 수 있다.

## 7. Commit 하기

깃허프 페이지는 *master branch* 에서 작업한 결과물이 posting 되는것 같다. github desktop 클라이언트에서 변경된 사항을 `commit`하고, `fetch` 하여 최종 결과물을 저장 및 동기화한다.
변경 사항이 있다면, `summary (required)`에 간단한 변경 내역을 작성해야 `commit` 버튼이 활성화된다.

## 8. Atom 에디터 사용하기

## 9. 패키지 설치하기
Markdown preview enhanced

## 10. LaTeX 사용하기

참고 사이트: <https://www.janmeppe.com/blog/How-to-add-mathjax-to-minimal-mistakes/>

Remote theme 인 minimal-mistakes의 [repository](https://github.com/mmistakes/minimal-mistakes)에서 `minimal-mistakes/_includes/scripts.html` 를 로컬 `_includes/scripts.html` 로 가져온다.

그리고 `scripts.html`에 아래의 스크립트를 추가한다.

``` HTML
<script type="text/javascript" async
	src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML">
</script>

<script type="text/x-mathjax-config">
   MathJax.Hub.Config({
     extensions: ["tex2jax.js"],
     jax: ["input/TeX", "output/HTML-CSS"],
     tex2jax: {
       inlineMath: [ ['$','$'], ["\\(","\\)"] ],
       displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
       processEscapes: true
     },
     "HTML-CSS": { availableFonts: ["TeX"] }
   });
</script>
```

> Note that this overrides any other include file in the remote theme.


## 11. TOC 사용하기

참고 사이트: <https://mmistakes.github.io/minimal-mistakes/docs/helpers/>

Front Matter에 다음을 넣는다

![toc](/assets/toc.png)

```
---
toc: true
toc_label: "My Table of Contents"
toc_icon: "cog"
---
```

## 12. 이미지 올리기
참고 사이트: <https://ahribori.com/article/5a03bcfd6c9eef13d882e29a>

이렇게 이슈로 링크를 올리고 나면, 이슈를 submit 하지 않고 닫아도 해당 링크 및 이미지가 계속 살아있다. ㄷㄷㄷ;;

```
[이미지 제목](링크)
```
git에 업로드한 이미지를 올리는 경우, 링크는 포스트(markdown 파일)가 위치한 곳을 root로 한 상대주소이다.
예를 들어,
![이미지 제목](/assets/ddd.JPG)
```
![이미지 제목](/assets/abc.JPG)
```
는 본 마크다운 포스트가 있는 폴더에 `assets`폴더가 있고, 해당 폴더 안에 `abc.jpg` 파일이 있다.

하지만, 포스팅 할 때는 이게 통하지 않는다. 아래와 같이 직접 링크를 따줘야 한다.
```
https://github.com/IcedVanillaLatte/IcedVanillaLatte.github.io/blob/master/_posts/assets/b.png?raw=true
```

github 클라이언트를 통해 commit & push 하지 않아도 Atom에서도 preview로 볼 수 있다.

github는 kromdown을 사용하기 때문에, 이미지 크기도 바꿀 수 있다. [참고 사이트](https://c10106.tistory.com/3363)

