---
layout: post
title: 'v6: JavaScripten'
tags: [hydejack]
description: >
  The last release made the theme fast in the eyes of Google, but not so much in the eyes of its readers.
  This release addresses this by adding a layer of JavaScript, effectively turning the whole site into a single page app.
redirect_from: /2017/04/15/javascripten-beta/
---

Hydejack has always featured a JavaScript-heavy sidebar, but other than that, JS has been used sparingly. This changes with this release, which adds a ton of (optional) code that changes the feel of the theme dramatically.

## Major
Pages are now loaded and swapped through JavaScript. This has a number of effects. First of all, it looks cool, but the animations aren't just about aesthetics: They also help to hide the network time of fetching the next page, making the entire site feel faster. At the same time, the FOUC introduced in the last release will no longer occur (except on the initial page load).

* Most JS is now unified in the `_js` directory and written in ES2016.
* The `blog-by-tag` layout has been renamed to `list`.
* `public` folder has been renamed to `assets` to make the theme compatible with Jekyll's gem-based themes.
* Tags are now supported via Jekyll Collections instead of `_data`.
* 사이드바에 이제 모든종류의 페이지 링크를 추가 할 수 있음
* 이제 카테고리들이 지원됨.
* 저자정보가 `_data/authors.yml` 로 이동됨
* Added support for multiple authors.
* Using `jekyll-feed` plugin (깃허브 Pages에서 지원되는) instead of custom solution.
* Added `about` layout.
* Added `not-found` layout.

See the [the migration guide]({{ site.baseurl }}{% link docs/6.0.0/migration.md %}) for instructions on how to upgrade.

## Minor

* The "accent" font (heading font) is now used for all headings. This gives the theme a "bolder" look and was necessary for the animation: link => heading.
* 기본 텍스트 "PT Serif" 에서 "Noto Serif" 로 바뀜
*  markdown컨텐츠 스타일링을 위한 [CSS classes]({{ site.baseurl }}{% link docs/6.0.0/writing.md %}) 추가
* 링크에 새로운 스타일 적용. 항상 밑줄로 표시 to make the choice of the link color less critical (어두운 색상이 일반 텍스트 보다 구분하기 힘들었음).
* 소셜미디어 아이콘을 크고 치기 쉽게 만듦
* 소셜미디어 아이콘이 이제 post 내 "about" 섹션의 한 부분이 되었음.
* Added support for a copyright notice at the bottom. Can be set via the config variable `copyright`.
* Changed responsive breakpoints and added support for very large displays.
* The site is now printable.
* The `blog` layout now only shows the excerpt instead of the full post.
* Links to external pages are now marked with a symbol.

## Fixes

* Related posts is no longer blank for posts that do not belong to a category.
* Footnotes now use the text version of "leftwards arrow with hook" instead of the emoji on iOS.
* Text is no longer invisible while waiting for Google Fonts to load.

***

[Get *JavaScripten* on GitHub](https://github.com/qwtel/hydejack/releases/tag/v6.0.0)

*[FOUC]: Flash of Unstyled Content
