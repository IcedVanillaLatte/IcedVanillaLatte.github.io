---
title: "(5) Upload images"
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake, Images]
toc: true
toc_sticky: true
published: true
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
---

이미지 포스팅을 위한 기본적인 마크다운 문법은 아래와 같다.
```
![image title](link)
```

## 이미지 링크 사용하기

내가 가진 이미지를 웹에 올려서 포스팅하는 경우 사용할 수 있는 방법이다.

GitHub의 *issue* 메뉴에서 클립보드에 있는 이미지를 붙여 넣으면, 아래와 같이 링크가 만들어진다. *Submit new issue* 버튼을 클릭하지 않고 닫아도 해당 이미지의 링크가 계속 살아있다. 

![image](https://user-images.githubusercontent.com/61964210/77402700-690a0900-6df2-11ea-9690-44726b57820e.png)

만들어진 마크다운 구문을 그대로 복사해서 붙여 넣으면 마크다운 형식으로 이미지가 삽입된다.
- 참고 사이트
	- <https://ahribori.com/article/5a03bcfd6c9eef13d882e29a>


## Repository 이미지 사용하기

내 repository에 올리는 경우, 이미지의 경로 주소는 내 repository를 root 경로로 사용한다.

Git에 업로드한 이미지를 올리는 경우, 링크는 포스트(markdown 파일)가 위치한 곳을 root로 한 상대주소이다.
예를 들어, `username.github.io/assets/images` 경로에 있는 `test.jpg` 파일은 아래와 같은 경로로 불러올 수 있다. 이때, 이미지의 경로 뒤에 **`?raw=true`** 를 꼭 붙여주자. 단순히 파일 이름만으로는 이미지가 올라오지 않는다.

``` markdown
![image](/assets/images/test.jpg?raw=true)
```

GitHub Page는 kramdown 문법을 지원하기 때문에, 첨부한 이미지의 크기를 `{: width="200", height="100"}
` 옵션으로 조절할 수 있다.
``` markdown
![image](/assets/images/test.jpg?raw=true){: width="200", height="100"}
```

- 참고사이트(kramdown 문법을 통한 이미지 크기 조절)
	- <https://c10106.tistory.com/3363>



<!--stackedit_data:
eyJoaXN0b3J5IjpbOTc1MjQzMTAwLDM3MDQxMDA1MF19
-->