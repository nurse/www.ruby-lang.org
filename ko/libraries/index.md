---
layout: page
title: "라이브러리"
lang: ko
---

대부분의 프로그레밍 언어와 마찬가지로 루비에서도 폭넓은 서드파티 라이브러리가
제공되고 있습니다.
{: .summary}

대부분의 서드파티 라이브러리들은 **젬**방식으로 배포되고 있습니다. [**RubyGems**][1]는
루비에 특화된 `apt-get`비슷한 분산 패키지 시스템으로 라이브러리의 작성이나 공개,
인스톨을 도와주는 시스템입니다. 루비 1.9 이후 버전부터 RubyGems는 루비에 표준첨부
되었습니다. 이전 버전의 루비에서는 [직접 인스톨][2] 할 필요가 있습니다.

그 외의 라이브러리는 **소스 코드** 디렉터리를 압축(.zip, .tar.gz)한 형태로 배포됩니다.
인스톨 방법은 다양하지만 보통 `README` 이나 `INSTALL`에 방법이 적혀있습니다.

라이브러리를 찾는 방법과 이를 설치하여 사용하는 것에 대해 알아봅니다.

### 라이브러리 찾기

루비의 라이브러리는 보동 [**RubyGems.org**][1]에서 젬으로 제공됩니다. 직접
웹사이트에서 둘러보거나 `gem`명령어로 이용할 수 있습니다.

`gem search -r`명령어를 사용해 RubyGems의 저장소를 조사할 수 있습니다. 예를 들어
`gem search -r rails`는 레일즈와 관련된 젬들의 목록을 돌려줍니다.
`--local` (`-l`) 옵션을 사용하면 인스톨된 들에대해 로컬 검색할 수 있습니다. 젬을
인스톨 하려면 `gem install [gem]`을 사용합니다. 인스톨된 젬을 보려면 `gem
list`를 사용합니다. 좀 더 정보가 필요하시면 아래 내용을 좀 더 읽으시거나 [RubyGems의
문서][3]를 참조하세요.

다른 라이브러리의 배포처도 있습니다. [RubyForge][4]는 예전엔 루비 라이브러리의
배포처로 널리 사용되었던 적이 있습니다. 하지만 최근 몇년간 [**GitHub**][5]가
루비 관련 라이브러리의 배포처로 대두되었습니다. 젬으로 RubyGems.org에
공개되어 있지만, 대부분의 젬의 소스코드는 GitHub에서 볼 수 있습니다.

[**The Ruby Toolbox**][6]는 오픈소스이며 루비 프로젝트를 검색하기 쉽게 하기 위한
프로젝트 입니다. 다양한 종류의 일반적인 개발 태스크를 카테고리로 릴리즈나 커밋의
활발함 라이브러리의 의존관계 등 각 프로젝트의 다양한 정보를 모았습니다. 또 RubyGems.org와
GitHub의 인기를 바탕으로 프로젝트의 순위를 매깁니다. 검색을 하면 원하는 것을 쉽게 찾으실
수 있을 것입니다.

### RubyGems에 대한 보충 설명

많이 쓰이는 `gem` 커맨드를 가볍게 보시려면, 이 패키지 관리시스템의 전반에
대한 [좀 더 자세한 문서][7]도 있습니다.

#### 젬 찾기

특정 이름으로 젬을 찾기 위해서는 **search** 명령을 사용합니다. 예를 들어 “html”이란 단어를 포함한 젬을 찾고
싶다면,

{% highlight sh %}
$ gem search -r html

*** REMOTE GEMS ***

html-sample (1.0, 1.1)
{% endhighlight %}

`--remote` / `-r` 플래그는 공식 RubyGems.org 저장소에서 검색하려 한다는
의미입니다. (기본 동작) `--local` / `-l` 플래그로는 인스톨된 젬에 대해
검색하게 됩니다.

#### 젬 설치하기

어떤 젬을 설치하기를 원한다면 **install** 명령을 사용합니다. 예를 들어 레일즈를
인스톨 하려면 이렇게 하면됩니다.

{% highlight sh %}
$ gem install rails
{% endhighlight %}

`--version` / `-v` 플래그를 이용하면 특정 버전을 지칭해서 설치할 수도 있습니다.

{% highlight sh %}
$ gem install rails --version 3.0
{% endhighlight %}

#### 모든 젬의 목록

현재 설치된 젬의 **목록**을 얻으려면 이렇게 하면 됩니다.

{% highlight sh %}
$ gem list
{% endhighlight %}


매우 길긴 하지만 RubyGems.org에 등록된 모든 젬의 **목록**을 볼 수도 있습니다.

{% highlight sh %}
$ gem list -r
{% endhighlight %}

#### Help!

터미널에서 문서를 열어볼 수 있습니다.

{% highlight sh %}
$ gem help
{% endhighlight %}

예를 들어 `gem help commands`는 모든 `gem`들의 커맨드를 볼 수 있어 매우 유용합니다.

#### Crafting your own gems

RubyGems.org에는 위의 주제들에 대한 [몇가지 가이드][3]가 있습니다. 덤으로
[Bundler][9]에 대해서 조사해보는 것도 도움이 되실 것 같습니다. Bundler는
RubyGems과 같이 일반적으로 사용되는 어플리케이션의 의존성 관리 툴입니다.



[1]: https://rubygems.org/
[2]: https://rubygems.org/pages/download/
[3]: http://guides.rubygems.org/
[4]: http://rubyforge.org/
[5]: https://github.com/
[6]: https://www.ruby-toolbox.com/
[7]: http://guides.rubygems.org/command-reference/
[9]: http://bundler.io/
