# Collaboration guide
[Mozzet](http://mozzet.com)의 제품 및 개발자 성장을 위한 협업 가이드라인입니다.

## Description
개발 과정은 **개발 전 설계 리뷰, 개발, 개발 후 코드 리뷰**의 과정을 거쳐 최종 반영되며, 총 두 단계의 리뷰를 두어 코드 퀄리티와 서비스의 안정성, 개발자들의 실력 향상을 목적으로 하고 있습니다.

## Plan Review
### How to
1. GitHub 저장소에 이슈를 올린다. 보통은 서버, 클라이언트 중 본인이 작업하는 플랫폼 저장소에 작성한다. 혹시 서버, 클라이언트 둘 다 적용되는 경우엔 서버 저장소에 작성한다.
2. Why, How, Weak Point의 3가지 틀에 맞춰 이 기능을 어떻게 개발할지 서술한다.
  1. **Why** - 문제, 원인, 왜 이 기능을 개발하였는지
  2. **How** - 어떻게, 어떤 방법으로 이 기능을 개발할 것인지 (최대한 구체적으로)
  3. **Weak Point** - 이 기능을 개발할 때 우려되는 점이 있다면 어떤 것인지
3. 브랜치로 구분하여 `feature`와 `hotfix` 각각 최소 3명, 2명의 리뷰어를 태그한다.
4. 리뷰를 받는 사람, 하는 사람 모두 입장을 명확하게 표현하며 이해가 안되는 부분이 있으면 바로바로 질문하여 모든 리뷰에 대한 답변이 이뤄질 수 있도록 한다.
5. 모든 리뷰가 끝났을 때 작성한 스펙에 맞게 개발을 시작한다.

## Code Review
### How to
1. Branch를 뗀다. (GitFlow Style의 `feature`, `hotfix` 두 가지 branch로)
3. `git diff` 를 활용해 코드 결과물을 최대한 명료하게, 커밋 메시지 또한 의미있게 작성한다.
4. branch에 알맞은 Label을 붙여 Pull Request를 올린다. 
5. 설계 리뷰에 리뷰를 담당했던 사람들은 다시 태그한다.
6. 설계 리뷰 이슈를 태그하고, 어떻게 테스트를 해볼 수 있는지에 대한 내용을 간단히 작성한 뒤 Pull Request를 올린다.
7. 리뷰를 받는 사람, 하는 사람 모두 입장을 명확하게 표현하며 이해가 안되는 부분이 있으면 바로바로 질문하여 모든 리뷰에 대한 답변이 이뤄질 수 있도록 한다.
8. 리뷰가 완료되면 본인이 Merge, 배포_(pullgy)_한다.

### 규칙
* 태그를 건 시점부터 24시간 내에 리뷰를 진행하는 것을 목표로 합니다.
* 매 개발팀 회의마다 1개 이상 내부적으로 공유할만한 리뷰를 가져옵니다.

## 개발자 지식 공유 Session
* 매주 한 명씩 약 15분 내외의 분량으로 기술 관련 발표를 진행합니다.
* 좋은 주제가 있다면 개발 블로그에 작성합니다.

## Style Guide

### PHP CodeIgniter
* **일반적으로 [CodeIgniter StyleGuide](https://ellislab.com/codeigniter/user-guide/general/styleguide.html)를 따릅니다.**
* WhiteSpace
	* `Space`가 아닌 `Tab`을 사용합니다.
* private method는 앞에 `_` 또한 붙여줍니다.

### HTML/CSS
* **일반적으로 [Google HTML/CSS Style Guide](http://google.github.io/styleguide/htmlcssguide.xml)를 따릅니다.**
* Indentation
	* 문서에서는 `2 Space`를 권장하나 개발 환경상 `Tab`으로 통일합니다.
* Template engine
	* [TWIG](http://twig.sensiolabs.org/)를 사용합니다.
* CSS Compiler
	* [less](http://lesscss.org/)를 사용합니다.

### Javascript
* **일반적으로 [Google JavaScript Style Guide](http://google.github.io/styleguide/javascriptguide.xml)를 따릅니다.**
* 객체 속성 접근은 온점(.)이 아닌 대괄호([])로 접근합니다.

### Android
* **일반적으로 [Google Java Style Guide](http://google.github.io/styleguide/javaguide.html)를 따릅니다.**

### Objective-C
* **기본적으로 [New York Times Objective-C Style Guide](https://github.com/NYTimes/objective-c-style-guide)를 따릅니다.**
	* Apple의 [Coding Guidelines for Cocoa](https://developer.apple.com/library/mac/documentation/Cocoa/Conceptual/CodingGuidelines/CodingGuidelines.html#//apple_ref/doc/uid/10000146-SW1)도 참고하면 좋습니다.