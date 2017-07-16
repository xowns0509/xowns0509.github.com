---
layout: post
title: Example content
tags: [hyde]
description: >
  안녕하신가! 이 예제포스트는 현재 테마가 지원하는 다양한 형태의 HTML컨텐트를 보여주고있다. 
author: mdo
---

Cum sociis natoque penatibus et magnis <a href="#">dis parturient montes</a>, nascetur ridiculus mus. *Aenean eu leo quam.* Pellentesque ornare sem lacinia quam venenatis vestibulum. Sed posuere consectetur est at lobortis. Cras mattis consectetur purus sit amet fermentum.

> Curabitur blandit tempus porttitor. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam id dolor id nibh ultricies vehicula ut id elit.

Etiam porta **sem malesuada magna** mollis euismod. Cras mattis consectetur purus sit amet fermentum. Aenean lacinia bibendum nulla sed consectetur.

## Inline HTML elements

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

- **글씨를 진하게 하려면 **, `**이렇게 양 옆에 별 2개씩 붙이세요**`.
- *이탤릭체를 원하면 *, `*이렇게 양 옆에 별 1개씩 붙이세요*`.
- 약어체(Abbreviations), like HTML should be defined like this `*[HTML]: HyperText Markup Language`.
- 인용구(Citations), like <cite>&mdash; Mark otto</cite>, should use `<cite>`.
- ~~취소선~~ 글씨는 `~~취소선~~` 으로 작성하시고 and <ins>밑줄</ins>은 `<ins>밑줄</ins>`태그로 열고 닫으세요.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

# Heading 1(머릿말 1단계)

## 머릿말 2단계
Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.

### 머릿말 3단계
Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor.

#### 머릿말 4단계
Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor.

##### 머릿말 5단계
Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor.

######머릿말 6단계
Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor.

## 코드인용

Cum sociis natoque penatibus et magnis dis `code element` montes, nascetur ridiculus mus.
코드를 작성하시고 물결표를 3개로 문단의 앞 뒤에 달아주세요.
~~~
코드내용
~~~

~~~js
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those
// arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
~~~

## 목록

아래와 같이 작성하면
~~~
* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Donec id elit non mi porta gravida at eget metus2
 * Nulla vitae elit libero, a pharetra augue.
   * Nulla vitae elit libero, a pharetra augue2
   * Nulla vitae elit libero, a pharetra augue3
~~~
이렇게 나타납니다.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Donec id elit non mi porta gravida at eget metus2
 * Nulla vitae elit libero, a pharetra augue.
   * Nulla vitae elit libero, a pharetra augue2
   * Nulla vitae elit libero, a pharetra augue3


항목 넘버링도 가능해요.
~~~
1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.
~~~
1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

Cras mattis consectetur purus sit amet fermentum. Sed posuere consectetur est at lobortis.

HyperText Markup Language (HTML)
: The language used to describe and define the content of a Web page

Cascading Style Sheets (CSS)
: Used to describe the appearance of Web content

JavaScript (JS)
: The programming language used to build advanced Web sites and applications

Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Nullam quis risus eget urna mollis ornare vel eu leo.

## 이미지

Quisque consequat sapien eget quam rhoncus, sit amet laoreet diam tempus. Aliquam aliquam metus erat, a pulvinar turpis suscipit at.

~~~
![800x400](https://placehold.it/800x400 "Large example image")
![400x200](https://placehold.it/400x200 "Medium example image")
![200x200](https://placehold.it/200x200 "Small example image")

~~~
![800x400](https://placehold.it/800x400 "Large example image")
![400x200](https://placehold.it/400x200 "Medium example image")
![200x200](https://placehold.it/200x200 "Small example image")

## 표

아래와 같이 작성하시면

~~~
| Name     | Upvotes   | Downvotes |
|:---------|:----------|:----------|
| Alice    |        10 |        11 |
| Bob      |         4 |         3 |
| Charlie  |         7 |         9 |
|==========|===========|===========|
|Totals    |        21 |        23 |
~~~

이렇게 나타납니다.
| Name     | Upvotes   | Downvotes |
|:---------|:----------|:----------|
| Alice    |        10 |        11 |
| Bob      |         4 |         3 |
| Charlie  |         7 |         9 |
|==========|===========|===========|
|Totals    |        21 |        23 |


*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets
*[JS]: JavaScript
