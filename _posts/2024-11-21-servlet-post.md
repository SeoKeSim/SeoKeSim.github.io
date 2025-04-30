---
layout: post
title: 서블릿 프로젝트
author: 김경환
tags: [overview, Servlet]
---

이 프로젝트는 넥슨 API를 활용하여 메이플스토리 게임의 캐릭터를 검색하고, 해당 캐릭터에 대한 다양한 정보를 제공하는 검색 및 가이드 기능을 구현한 시스템입니다. 사용자는 자신의 게임 캐릭터를 쉽게 검색하여 레벨, 직업, 아이템 정보 등 다양한 정보를 확인할 수 있습니다. 또한, 게임 내의 컨텐츠 추천 및 가이드를 제공하여, 플레이어가 보다 효율적으로 게임을 즐길 수 있도록 도와줍니다.

# 메인 기능

### 회원가입 기능
사용자는 자신의 계정을 생성하여, 저장된 캐릭터 정보를 안전하게 관리하고, 나만의 게임 데이터를 기록할 수 있습니다. 회원가입 후에는 개인화된 서비스를 제공받을 수 있습니다.

### NEXON API를 활용한 캐릭터 검색 기능
넥슨의 공식 API를 통해 메이플스토리 캐릭터의 정보를 실시간으로 검색할 수 있습니다. 

### 캐릭터 정보 확인
캐릭터의 레벨, 직업, 아이템 등 다양한 게임 데이터를 한눈에 확인할 수 있습니다. 이를 통해 사용자는 자신의 캐릭터 상태를 빠르게 확인 가능합니다.

### 캐릭터 장비 확인
사용자는 자신의 캐릭터가 착용하고 있는 장비 정보(무기, 방어구, 악세서리 등)를 확인할 수 있습니다. 이 기능은 장비 업그레이드나 개선에 필요한 참고 자료를 제공합니다.

### 게임 내 가이드 제공
캐릭터의 레벨, 직업, 아이템 등을 기반으로 게임 플레이에 유용한 가이드를 자동으로 제공합니다. 현재 전투력을 기반으로 보스 몬스터 가이드를 제공 하고 있습니다.

## Lists

Unordered:

- Fusce non velit cursus ligula mattis convallis vel at metus[^2].
- Sed pharetra tellus massa, non elementum eros vulputate non.
- Suspendisse potenti.

Ordered:

1. Quisque arcu felis, laoreet vel accumsan sit amet, fermentum at nunc.
2. Sed massa quam, auctor in eros quis, porttitor tincidunt orci.
3. Nulla convallis id sapien ornare viverra.
4. Nam a est eget ligula pellentesque posuere.

## Blockquote

The following is a blockquote:

> Suspendisse tempus dolor nec risus sodales posuere. Proin dui dui, mollis a consectetur molestie, lobortis vitae tellus.

## Thematic breaks (<hr>)

Mauris viverra dictum ultricies[^3]. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **You can put some text inside the horizontal rule like so.**

---
{: data-content="hr with text"}

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **Or you can just have an clean horizontal rule.**

---

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. Or you can just have an clean horizontal rule.

## Code

Now some code:

```
const ultimateTruth = 'follow middlepath';
console.log(ultimateTruth);
```

And here is some `inline code`!

## Tables

Now a table:

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

## Images

![theme logo](http://www.abhinavsaxena.com/images/abhinav.jpeg)

This is an image[^4]

---
{: data-content="footnotes"}

[^1]: this is a footnote. You should reach here if you click on the corresponding superscript number.
[^2]: hey there, don't forget to read all the footnotes!
[^3]: this is another footnote.
[^4]: this is a very very long footnote to test if a very very long footnote brings some problems or not; hope that there are no problems but you know sometimes problems arise from nowhere.
