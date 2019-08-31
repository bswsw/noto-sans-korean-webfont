# Noto Sans Korean for Web Developer

[![GitHub version](https://badge.fury.io/gh/andrewbae%2Fnoto-sans-korean-webfont.svg)](https://badge.fury.io/gh/andrewbae%2Fnoto-sans-korean-webfont)
[![Bower version](https://badge.fury.io/bo/noto-sans-korean-webfont.svg)](https://badge.fury.io/bo/noto-sans-korean-webfont)

`noto-sans-korean-webfont`는 웹 개발자를 위한 본고딕(Noto Sans Korean) 웹폰트 입니다.
- 경량화된 폰트를 사용하여 빠른 속도로 로딩이 가능합니다. (약 `6.3MB`)
- `.css`, `.scss` 모두 제공하여 입맛대로 사용할 수 있습니다.

## 사용 가이드 (Usage)

직접 다운로드 하거나 `bower`를 이용할 수 있어요.

* [Download](#1-download)
* [Bower](#2-bower)

### 1. Download

다운로드 받으셨다면 먼저 사용할 프로젝트의 원하는 경로에 넣어주세요.

#### 1.1. CSS 사용하기

사용하는 메인 `.css` 파일 상단에 다음과 같이 입력하세요.

```css
/** css 파일 가져오기 */
@import("path/noto-sans-korean-webfont/css/noto-sans-korean.css");

/**
 * body에 폰트 적용.
 * 부분만 적용하고 싶으면 필요한 곳에 적용.
 */
body {
  font-family: "Noto Sans Korean", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

##### 주의사항

- 다운받은 폴더의 경로를 정확히 확인해 주세요.
- 내부의 폴더 (`css/`, `fonts/`) 경로를 이동할 경우  `css/noto-sans-korean.css` 파일에서 경로를 이동한 경로로 변경해 주어야 해요.

#### 1.2. SCSS 사용하기

사용하는 메인 `.scss` 파일 상단에 다음과 같이 입력하세요.

```sass
// fonts 폴더 경로 추가.
$noto-sans-korean-path: "path/noto-sans-korean-webfont/fonts/";

// _noto-sans-korean.sass 파일 경로 추가.
@import "path/noto-sans-korean-webfont/scss/noto-sans-korean";

// body에 폰트 적용
// 부분만 적용하고 싶으면 필요한 곳에 적용.
body {
  font-family: "Noto Sans Korean", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

##### 주의사항

- 다운받은 폴더의 경로를 정확히 확인해 주세요.
- `scss/`, `fonts/` 폴더의 위치를 마음대로 설정하셔도 `$noto-sans-korean-path`와 `scss/_noto-sans-korean.scss`만 `@import`를 정확히 해주시면 문제는 없을거에요.

### 2. Bower

Bower Package를 받으세요.

```console
$ bower install --save noto-sans-korean-webfont
```

#### 2.1. CSS 사용하기

사용하는 메인 `.css` 파일 상단에 다음과 같이 입력하세요.

```css
/** css 파일 가져오기 */
@import("bower_components/noto-sans-korean-webfont/css/noto-sans-korean.css");

/**
 * body에 폰트 적용.
 * 부분만 적용하고 싶으면 필요한 곳에 적용.
 */
body {
  font-family: "Noto Sans Korean", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

#### 2.2. SCSS 사용하기

사용하는 메인 `.scss` 파일 상단에 다음과 같이 입력하세요.

```sass
// fonts 폴더 경로 추가.
$noto-sans-korean-path: "../bower_components/noto-sans-korean-webfont/fonts/";

// sass 파일 경로 추가.
@import "../bower_components/noto-sans-korean-webfont/scss/noto-sans-korean";

// body에 폰트 적용
// 부분만 적용하고 싶으면 필요한 곳에 적용.
body {
  font-family: "Noto Sans Korean", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

#### 2.3. Bower로 설치시 주의사항
- 메인 `.scss` 파일의 경로와 `bower_components`의 상대 경로를 정확히 확인해 주세요.
- `gulp` 혹은 `grunt` 등 빌드 자동화 툴을 사용할 경우 각자 환경에 맞춰 이용해 주세요.

## 폰트 출처 및 라이센스
Noto Sans는 Google과 어도비가 합작해 개발한 웹폰트입니다. 라이센스는 [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html) 입니다.
- [Google Noto Fonts](https://www.google.com/get/noto/#/)
- [NotoSans-subset](https://github.com/UYEONG/NotoSans-subset)

## 개발자 한마디
- 자유롭게 사용해 주세요.
- 부족한 점이 많아요. 개선할 부분이 있다면 언제든지 가르침을 주세요.
- 개발자 분들 모두 힘내세요!

