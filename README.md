# code-style-guide
Mozzet의 제품 및 개발자 성장을 위한 개발 코드 가이드라인입니다.  
코드 가이드의 경우 기반을 두는 문서 외에 자주 언급되는 부분들은 다시 명시하였습니다.  
**수정은 개발자 회의를 거쳐 적용됨을 알아주세요.**  
이 Guide는 `2015.10.07`에 작성되었으며, `2015.10.xx`부터 시행 예정입니다.

## Code Review
### How to
1. Branch를 뗀다. (GitFlow Style의 `feature`, `hotfix` 두 가지 branch로)
2. 개발
3. `git diff` 로 최대한 명료하게, 커밋 메시지 또한 의미있게
4. Pull Request를 올린다.
5. `feature`는 2명, `hotfix`는 1명의 리뷰어를 태그
6. 리뷰가 완료되면 본인이 Merge, 배포(pullgy)

### 규칙
* 개발 팀장님이신 만기님은 현재 모든 리뷰에 참여합니다. 만기님을 제외하고 태그해주세요.
* 태그를 건 시점부터 최대 24시간 내에 리뷰를 진행합니다.

## 개발자 지식 공유 Session
* 2주에 한 명씩 약 15분 내외의 분량으로 기술 관련 발표를 진행합니다.
* 좋은 주제가 있다면 개발 블로그 작성 준비합니다.

## Style Guide

### PHP CodeIgniter
* **일반적으로 [CodeIgniter StyleGuide](https://ellislab.com/codeigniter/user-guide/general/styleguide.html)를 따릅니다.**
* WhiteSpace
	* `Space`가 아닌 `Tab`을 사용합니다.

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

### Android
* **일반적으로 [Google Java Style Guide](http://google.github.io/styleguide/javaguide.html)를 따릅니다.**

### iOS
* **일반적으로 [Google Objective-C Style Guide](http://google.github.io/styleguide/objcguide.xml)를 따릅니다.**
	* Apple의 [Coding Guidelines for Cocoa](https://developer.apple.com/library/mac/documentation/Cocoa/Conceptual/CodingGuidelines/CodingGuidelines.html#//apple_ref/doc/uid/10000146-SW1)도 참고하면 좋습니다.