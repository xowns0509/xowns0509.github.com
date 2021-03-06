---
layout: post
title: Hydejack을 소개합니다.
tags: [hydejack]
description: >
  Introducing Hydejack 내용을 일부 한글로 번역해 봄.

---

***

## 특징
Unlike Hyde, it's very opinionated about how you are going to use it.

Features include:

* 리스트를 만들려면 별(아스테릭) 1개
* 터치 가능한 사이드바 / 모바일에선 서랍형, including fallback when JS is disabled
* Github Pages compatible tag support based on [this post][tag].
* 조정가능한 링크색상과 사이드바 이미지, 사이트 마다, 태그 마다, 포스트 마다
* 포스트의 하단에 위치한 선택적 저자섹션
* 선택적 댓글 섹션 powered by Disqus.
* 년도별 포스트 레이아웃
* 사이드바에 위치한 Wide array of 소셜미디어 아이콘
* Math blocks via [KaTeX](https://khan.github.io/KaTeX/).

## 다운로드
Hydejack은 GitHub에 의해 개발되고 호스트됨. Head to the [GitHub repository](https://github.com/qwtel/hydejack) for downloads, bug reports, and feature requests.

## 사이드바
I love the original Hyde theme, but unfortunately the layout isn't as great on small screens.
Since the sidebar moves to the top, the user has to scroll down just to read the title of a blog post.

By using a drawer component I was able to retain the original two column layout. It's possible to move the drawer via touch input (with the help of a little JavaScript).

Since the background image contributes to the feel of the page I'm letting it peek over the edge a bit. This also provides a hint to the user that an interaction is possible.

## 설명서

### 설정하기
[`_config.yml`](https://github.com/qwtel/hydejack/blob/v3/_config.yml)를 통해 중요한 부분을 설정할 수 있다. This includes:

* 사이드바의 블로그 설명
* (선택적) 저자설명과 저자의 사진
* 블로그의 기본이미지와 링크색상
* 깃허브와 트위터 사용자명

### 포스트의 색상과 이미지 바꾸는 방법
In the manifest of a blog post,`image`로 url이나  `color`로 CSS 색상을 간단하게 추가:

~~~yml
layout: post
title: Introducing Hydejack
image: https://qwtel.com/hydejack/assets/img/hyde.jpg
color: '#949667'

물결 셋
~~~

### 태그 추가하기
Tags are not meant to be used #instagram #style: #food #goodfood #happy #happylife #didimentionfood #yougetthepoint, as each tag requires some setup work. I tend to think of it as categories that can be combined.

1.  Add an entry to `_data/tags.yml`, where the key represents a slug and provide at least a `name` value and optionally `image`, `color` and `description`.

    Example `/_data/tags.yml`:

    ~~~yml
    mytag:
      name: My Tag
    ~~~

2.  Make a new file in the `tag` folder, using the same name you've used as the key / slug and change the `tag` and `permalink` entries.

    Example `/tag/mytag.md`:

    ~~~yml
    layout: blog-by-tag
    tag: mytag
    permalink: /tag/mytag/
    ~~~

3.  Tag your blog posts using the `tags` key (color and image will only depend on the first tag).

    ~~~yml
    layout: post
    title: Introducing My New Tag
    tags: [mytag, othertag]
    ~~~

4. (optional) Add the tag to the sidebar, by adding it to `sidebar_tags` in `_config.yml`.
   They will appear in the listed order.

   ~~~yml
   sidebar_tags: [mytag, othertag]
   ~~~

[tag]: http://www.minddust.com/post/tags-and-categories-on-github-pages/
