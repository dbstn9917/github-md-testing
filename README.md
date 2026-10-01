# Post.scss

일관된 **Post** 스타일, **class** 하나로 딸깍!

Post, Article, Docs 등 웹 문서에 일관되고 깔끔한 스타일이 필요하다면 **Post.scss**를 적용해 보세요.  
한 번에 컨테이너 내부의 모든 요소에 스타일을 적용하거나, 개별 요소에 스타일을 적용할 수 있습니다.  
요소의 스타일을 간편하게 제거하거나, Post 스타일을 커스터마이징할 수도 있습니다.

## 시작하기

1. `scss/` 폴더를 다운로드한 뒤 해당 폴더를 프로젝트에 불러옵니다.
2. `post.scss` 파일을 컴파일해 준 뒤, HTML 문서에 `<link>` 태그로 첨부해 줍니다.
3. 스타일 적용이 필요한 요소를 감싸는 부모 컨테이너에 `post--container` 클래스를 부여합니다.

## Post 스타일

Post.scss로 적용한 **Post 스타일**은 다음의 특징을 갖고 있습니다.

1. 문서의 요소들을 보기 편하게 꾸며줍니다.
2. WHATWG의 HTML 표준을 참조해 만들었습니다.
3. 대부분의 스타일이 `em`, `rem` 단위를 사용해 부모 요소의 `font-size`를 변경하는 것으로 하위 요소들의 크기를 간편하게 수정할 수 있습니다.

## Post container

`post--container` 클래스를 부여하면 컨테이너 내부의 요소들에 Post 스타일을 일괄적으로 적용할 수 있습니다.

```html
<div class="post--container">
  <p><strong>Post 스타일</strong>을 적용해 보세요!</p>
</div>
```

## inline Post class

`post--container` 외부에서도 특정 요소에 Post 스타일을 적용할 수 있습니다.

```html
<p>언제든 <mark class="post--mark">필요할 때</mark> Post 스타일 불러오기</p>
```

**inline Post class**로 Post 스타일을 적용하고 싶으면 `post--[태그 이름]` 형태로 클래스를 부여하면 됩니다.

**inline Post class**가 부여된 요소는 Post 스타일이 적용되지만, 내부의 하위 요소들은 스타일이 적용되지 않습니다. 따라서 내부 요소에도 스타일을 적용하고 싶다면 개별 요소에 **inline Post class**를 부여하거나, **Post container**를 이용해 주세요

## Post disable

`post--disable` 클래스를 부여하면 요소의 Post 스타일을 비활성화합니다.

```html
<div class="post--container">
  <p class="post--disable">Post 스타일을 비활성화해 보세요!</p>
</div>
```

`post--disable` 클래스가 부여된 요소의 하위 요소 또한 Post 스타일이 비활성화됩니다.

## Copyright

Copyright © 2026 Dopamintic. All rights reserved.
