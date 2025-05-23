---
layout: post
title: 서블릿 프로젝트
author: 김경환
tags: [overview, Servlet]
---

이 프로젝트는 3명이서 협업하여 진행되었으며, 저는 **넥슨 API 연동 및 기능 구현**을 담당했습니다.<br>
메이플스토리 캐릭터 검색 및 가이드 시스템을 구현하여, 사용자가 캐릭터 정보(레벨, 직업, 아이템 등)를 쉽게 확인하고, 게임 내 컨텐츠 추천 및 가이드를 받을 수 있도록 설계하였습니다.

<!-- 이 프로젝트는 3명이서 협업 하여 진행 하였습니다. 저는 넥슨 API 연동 및 기능 구현을 주로 담당하였습니다. <br> 넥슨 API를 활용하여 메이플스토리 게임의 캐릭터를 검색하고, 해당 캐릭터에 대한 다양한 정보를 제공하는 검색 및 가이드 기능을 구현한 시스템입니다.<br> 사용자는 자신의 게임 캐릭터를 쉽게 검색하여 레벨, 직업, 아이템 정보 등 다양한 정보를 확인할 수 있습니다.<br> 또한 게임 내의 컨텐츠 추천 및 가이드를 제공하여, 플레이어가 보다 효율적으로 게임을 즐길 수 있도록 도와주도록 설계 하였습니다.  -->

# 메인 기능

### - 회원가입 기능
사용자는 자신의 계정을 생성하여, 저장된 캐릭터 정보를 안전하게 관리하고, 나만의 게임 데이터를 기록할 수 있습니다.<br> 회원가입 후에는 캐릭터 즐겨찾기 서비스를 제공받을 수 있습니다.

### - NEXON API를 활용한 캐릭터 검색 기능
넥슨의 공식 API를 통해 메이플스토리 캐릭터의 정보를 실시간으로 검색할 수 있습니다. 

### - 캐릭터 정보 확인
캐릭터의 레벨, 직업, 아이템 등 다양한 게임 데이터를 한눈에 확인할 수 있습니다. <br> 이를 통해 사용자는 자신의 캐릭터 상태를 빠르게 확인 가능합니다.

### - 캐릭터 장비 확인
사용자는 자신의 캐릭터가 착용하고 있는 장비 정보(무기, 방어구, 악세서리 등)를 확인할 수 있습니다. <br>이 기능은 장비 업그레이드나 개선에 필요한 참고 자료를 제공합니다.

### - 게임 내 가이드 제공
캐릭터의 레벨, 직업, 아이템 등을 기반으로 게임 플레이에 유용한 가이드를 자동으로 제공합니다. <br>현재 전투력을 기반으로 보스 몬스터 가이드를 제공 하고 있습니다.

# SkillSet

#### 관련기술

- JavaScript – API 호출 및 동적 데이터 처리
- HTML/CSS – UI 구조 및 스타일링
- Nexon Open API – 메이플스토리 캐릭터 정보 제공
- Git / GitHub – 버전 관리 및 배포


#### 개발 도구

- Eclipse – Java 백엔드 및 서블릿 개발 환경
- Visual Studio Code (VS Code) – 정적 페이지(HTML, CSS, JS) 편집

# 컨트롤러 핵심 기능

### usercontroller
<button class="accordion">UserController</button>
<div class="panel">
    <pre><code>
public class UserController {
    // 사용자 관련 API 처리
    @GetMapping("/user/{id}")
    public User getUser(@PathVariable Long id) {
        return userService.findById(id);
    }
}
    </code></pre>
</div>

# Thematic breaks (<hr>)

Mauris viverra dictum ultricies[^3]. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **You can put some text inside the horizontal rule like so.**

---
{: data-content="hr with text"}

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **Or you can just have an clean horizontal rule.**

---

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. Or you can just have an clean horizontal rule.

# Code

Now some code:

```
const ultimateTruth = 'follow middlepath';
console.log(ultimateTruth);
```

And here is some `inline code`!

# DB Tables

Now a table:

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

# 사이트 구성

![theme logo](http://www.abhinavsaxena.com/images/abhinav.jpeg)

This is an image[^4]

---

<!-- JavaScript for accordion functionality -->
<script>
    var acc = document.getElementsByClassName("accordion");
    for (var i = 0; i < acc.length; i++) {
        acc[i].addEventListener("click", function() {
            this.classList.toggle("active");
            var panel = this.nextElementSibling;
            if (panel.style.display === "block") {
                panel.style.display = "none";
            } else {
                panel.style.display = "block";
            }
        });
    }
</script>