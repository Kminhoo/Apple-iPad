# 🍎Apple-iPad
이 프로젝트는 애플(아이패드) 홈페이지를 클론코딩한 프로젝트 입니다.
HTML, CSS, JS를 사용해서 구현하였습니다.
 

[완성본](https://i-pad-with-fastcampus.vercel.app/)



![appleipad](https://github.com/Kminhoo/Apple-iPad/assets/102332763/a8af724e-d602-4bc2-8275-90394b915551)



## 프로젝트 소개
- 이 프로젝트는 웹 개발 학습의 심화를 다지기 위해 진행했습니다.
- 기존의 애플-아이패드 홈페이지의 기능와 디자인을 최대한 재현하려 노력했습니다.
- 반응형 웹 디자인을 적용하여 다양한 디바이스에서 원할하게 이용할 수 있습니다.

<br />
<br />

## 학습 내용 
- HTML5
### twitter card 와 Open Graph 를 이용한 소셜미디어 공유 정보
```html
<!-- open Graph -->
<meta property="og:type" content="website" />
<meta property="og:site_name" content="Apple (KR)" />
<meta property="og:title" content="iPad 10.2" />
<meta property="og:description" content="강력한 A13 Bionic 칩을 탑재한 iPad. 센터 스테이지 기술이 적용된 12MP 울트라 와이드 전면 카메라, True Tone 디스플레이 기술 및 64GB 저장 용량까지 갖췄습니다." />
<meta property="og:image" content="./images/ipad-seo.png" />
<meta property="og:url" content="https://www.apple.com/kr/ipad-10.2" />

<!-- twitter card -->
<meta property="twitter:card" content="surmmary" />
<meta property="twitter:site" content="Apple (KR)" />
<meta property="twitter:title" content="iPad 10.2" />
<meta property="twitter:description" content="강력한 A13 Bionic 칩을 탑재한 iPad. 센터 스테이지 기술이 적용된 12MP 울트라 와이드 전면 카메라, True Tone 디스플레이 기술 및 64GB 저장 용량까지 갖췄습니다." />
<meta property="twitter:image" content="./images/ipad-seo.png" />
<meta property="twitter:url" content="https://www.apple.com/kr/ipad-10.2" />
```
twitter card 와 Open Graph를 이용한 소셜미디어 공유 정보에 대해 공유되는 내용을 추가
<br />
<br />
### reset cdn을 사용한 css 초기화
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css" />
```
reset cdn 을 사용하여 브라우저마다 차이가 있는 기본스타일을 초기화하고, 다양한 브라우저에서 동일한 레이아웃을 보여주려 했습니다.
<br />
<br />

- CSS
### 변수를 사용한 css 스타일링
```css
html {
  --color-white: #fff;
  --color-black: #000;  
  --color-font: #1d1d1d;
  --color-font-darkgray: #6e6e6e;
  --color-font-middlegray: #b7b7b7;
  --color-font-lightgray: #f5f5f5;
  --color-link: #0071e3;
  --color-link-focus: #81b9f1;
  --color-border: #d2d2d2;
  --color-header: #3a3a3a;
  --color-section: #f5f5f5;
  --color-shadow: rgba(0, 0, 0, .4);
}
```
자주 사용하는 색상을 변수로 선언하여 재사용성을 높이고, 유지보수를 쉽게 할 수 있게 했습니다. <br /> 
선언한 변수에 의미를 두어 읽기 쉽게 했습니다. 
<br/>

```css
@media (max-width: 1000px) {
    .inner {
        max-width: 692px;
    }
}

@media (max-width: 740px) {
    .links {
        flex-direction: column;
        align-items: center;
        gap: 16px;
    }
    a.link {
        font-size: 17px;
    }
}
```
@meida Query를 사용한 반응형 웹 디자인 적용했습니다. <br />
break point를 max-wdith로 사용하여 1000px, 768px 태블릿과, 모바일에 적용했습니다.

<br />
<br />

- JavaScript

DOM 조작, 이벤트핸들러, 내장객체 등 Javascript의 내용을 사용했습니다. <br />
JSON Data 형식을 공부하고, 사용하는 방법에 대해 이해하고 공부했습니다. <br />
메소드체이닝을 사용하여 코드의 가독성을 높였습니다.

<br/>
<br/>

- 배포

Vercel을 통해 정적인 웹사이트 배포하는 방법에 대해 공부했습니다.

