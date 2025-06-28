---
title: "(4) Latex Expression"
categories: [GitHub Page]
tags: [GitHub, Minimal Mistake, Latex]
toc: true
toc_sticky: true
published: true
sidebar:
  title: "GitHub Page 따라하기"
  nav: github
---

## LaTeX Script


Remote theme 인 minimal-mistakes의 [repository](https://github.com/mmistakes/minimal-mistakes)에서 `minimal-mistakes/_includes/scripts.html` 를 로컬 `_includes/scripts.html` 로 가져온다.

그리고 `scripts.html`에 아래의 스크립트를 추가한다.

``` html
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


- 참고 사이트
	- <https://www.janmeppe.com/blog/How-to-add-mathjax-to-minimal-mistakes/>{: target="_blank"}


## Example : LaTeX Equation Expression


GitHub page에서 위 스크립트가 정상적으로 로드되었다면, 아래와 같은 방법으로 LaTex 수식을 표현할 수 있다.

|Syntax|Expression|
|:---:|:---:|
|`$x = y$`|$x = y$|
|`$x < y$`|$x < y$|
|`$x > y$`|$x > y$|
|`$x \le y$`|$x \le y$|
|`$x \ge y$`|$x \ge y$|
|`$x^{n}$`|$x^{n}$|
|`$x_{n}$`|$x_{n}$|
|`$\overline{x}$`|$\overline{x}$|
|`$\hat{x}$`|$\hat{x}$|
|`$\tilde{x}$`|$\tilde{x}$|
|`$\frac{a}{b}$`|$\frac{a}{b}$|
|`$\displaystyle \frac{a}{b}$`|$\displaystyle \frac{a}{b}$|
|`$\binom{n}{k}$`|$\binom{n}{k}$|
|`$x_{1} + x_{2} + \cdots + x_{n}$`|$x_{1} + x_{2} + \cdots + x_{n}$|
|`$x_{1}, x_{2}, \dots, x_{n}$`|$x_{1}, x_{2}, \dots, x_{n}$|
|`$\mathbf{x}=\langle x_{1},x_{2},\dots,x_{n}\rangle$`|$\mathbf{x}=\langle x_{1},x_{2},\dots,x_{n}\rangle$|
|`$|A|$`| \|$A$\| |
|`$\|A\|$` | $\|A\|$ |
|`$x \in A$`|$x \in A$|
|`$x \subset B$`| $x \subset B$|
|`$x \subseteq B$`|$x \subseteq B$|
|`$A \cup B$`|$A \cup B$|
|`$A \cap B$`|$A \cap B$|
|`$X \sim {\sf Binom}(n, \pi)$`  |$X \sim {\sf Binom}(n, \pi)$|
|`$P(A \mid B)$`|$P(A \mid B)$|
|`$\{1, 2, 3\}$`|$\{1, 2, 3\}$|
|`$\sin(x)$`|$\sin(x)$|
|`$\log(x)$`|$\log(x)$|
|`$\sum_{n=1}^{10} n^2$`|$\sum_{n=1}^{10} n^2$|
|`$$\sum_{n=1}^{10} n^2$$`|$$\sum_{n=1}^{10} n^2$$|
|`$$\sum_x=1^10 x^2$$`|$$\sum_x=1^10 x^2$$|
|`$X \sim {\sf Binom}(n, \pi)$`|$X \sim {\sf Binom}(n, \pi)$|
|`$\int_{a}^{b}$`|$\int_{a}^{b}$|
|`$\left(\int_{a}^{b} f(x) \; dx\right)$`|$\left(\int_{a}^{b} f(x) \; dx\right)$|
|`$\left[\int_{-\infty}^{\infty} f(x) \; dx\right]$`|$\left[\int_{-\infty}^{\infty} f(x) \; dx\right]$|
|`$\left. F(x) \right|_{a}^{b}$`|$\left. F(x) \right\|_{a}^{b}$|
|`$\sum_{x = a}^{b} f(x)$`|$\sum_{x = a}^{b} f(x)$|
|`$\prod_{x = a}^{b} f(x)$`|$\prod_{x = a}^{b} f(x)$|
|`$\lim_{x \to \infty} f(x)$`|$\lim_{x \to \infty} f(x)$|
|`$\displaystyle \lim_{x \to \infty} f(x)$`|$\displaystyle \lim_{x \to \infty} f(x)$|



## Greek Letters

|Syntax|Expression|
|:---:|:---:|
|`$\alpha A$`|$\alpha A$|
|`$\nu N$`|$\nu N$|
|`$\beta B$`|$\beta B$|
|`$\xi\Xi$`|$\xi\Xi$|
|`$\gamma \Gamma$`|$\gamma \Gamma$|
|`$o O$` (omicron)|$o O$|
|`$\delta \Delta$`|$\delta \Delta$|
|`$\pi \Pi$`|$\pi \Pi$|
|`$\epsilon \varepsilon E$`|$\epsilon \varepsilon E$|
|`$\rho\varrho P$`|$\rho\varrho P$|
|`$\zeta Z \sigma$`|$\zeta Z \sigma$|
|`$\sigma \Sigma$`|$\sigma \Sigma$|
|`$\eta H$`|$\eta H$|
|`$\tau T$`|$\tau T$|
|`$\theta \vartheta \Theta$`|$\theta \vartheta \Theta$|
|`$\upsilon \Upsilon$`|$\upsilon \Upsilon$|
|`$\iota I$`|$\iota I$|
|`$\phi \varphi \Phi$`|$\phi \varphi \Phi$|
|`$\kappa K$`|$\kappa K$|
|`$\chi X$`|$\chi X$|
|`$\lambda \Lambda$`|$\lambda \Lambda$|
|`$\psi \Psi$`|$\psi \Psi$|
|`$\mu M$`|$\mu M$|
|`$\omega \Omega$`|$\omega \Omega$|


- 참고 사이트 : <https://www.calvin.edu/~rpruim/courses/s341/S17/from-class/MathinRmd.html>




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYyMTYyNjE3NywtMTc1MDAyNTg3LDgxMT
gxMjA2NywtMzk4MDcyMzAzLC0xOTc4NDA1MzU5XX0=
-->