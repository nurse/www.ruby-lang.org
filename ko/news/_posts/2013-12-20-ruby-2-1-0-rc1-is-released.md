---
layout: news_post
title: "Ruby 2.1.0-rc1 릴리즈"
author: "nurse"
translator: "marocchino"
date: 2013-12-20 16:53:05 +0000
lang: ko
---

Ruby 2.1.0-rc1 를 릴리즈 했습니다.
2013/12/25 로 예정되어있는 최종 릴리즈 전에 신기능을 시험해보세요.

## preview2 이후의 주목할만한 변경점

* 확장 라이브러리 curses 의 삭제 [#8584](https://bugs.ruby-lang.org/issues/8584)

그밖의 변경은 [NEWS](https://github.com/ruby/ruby/blob/v2_1_0_rc1/NEWS) 를 참고해 주세요.

## 다운로드

* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.tar.bz2](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.tar.bz2)
  * SIZE:   11394226 bytes
  * MD5:    cae095b90349b5b0f7026060cc3dd2c5
  * SHA256: af828bc0fe6aee5ffad0f8f10b48ee25964f54d5118570937ac7cf1c1df0edd3
* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.tar.gz](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.tar.gz)
  * SIZE:   14450990 bytes
  * MD5:    a16561f64d78a902fab08693a300df98
  * SHA256: 1b467f13be6d3b3648a4de76b34b748781fe4f504a19c08ffa348c75dd62635e
* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.zip](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-rc1.zip)
  * SIZE:   16107702 bytes
  * MD5:    b6cdc0e63185b4aeb268bdf6ebd4de9f
  * SHA256: 4d6a256b73b79f5b64182e1f55db3e61042bbe0166a45917e69c1b4e47247276

## 2.0 이후의 변경점

Ruby 2.0.0 이후의 주목할반한 변경은 다음과 같습니다.

* VM (메소드 케쉬)
* RGenGC (ko1님의 [RubyKaigi 프리젠테이션](http://rubykaigi.org/2013/talk/S73) 과 [RubyConf 2013 프리젠테이션](http://www.atdot.net/~ko1/activities/rubyconf2013-ko1_pub.pdf)을 확인하세요)
* refinements [#8481](https://bugs.ruby-lang.org/issues/8481) [#8571](https://bugs.ruby-lang.org/issues/8571)
* 문법의 변경
  * Rational/Complex 리터럴 [#8430](https://bugs.ruby-lang.org/issues/8430)
  * def 의 리턴 치 [#3753](https://bugs.ruby-lang.org/issues/3753)
* Bignum
  * GMP 의 사용 [#8796](https://bugs.ruby-lang.org/issues/8796)
* String#scrub [#8414](https://bugs.ruby-lang.org/issues/8414)
* Socket.getifaddrs [#8368](https://bugs.ruby-lang.org/issues/8368)
* RDoc 4.1.0 과 RubyGems 2.2.0
* "literal".freeze 의 최적화 [#9042](https://bugs.ruby-lang.org/issues/9042)
* Exception#cause 의 추가 [#8257](https://bugs.ruby-lang.org/issues/8257)
* 라이브러리 업데이트: BigDecimal, JSON, NKF, Rake, RubyGems, RDoc
* 확장라이브러리 curses 의 삭제 [#8584](https://bugs.ruby-lang.org/issues/8584)

더 자세한 변경점은 [Ruby 레포지터리의 NEWS (작업중)](https://github.com/ruby/ruby/blob/v2_1_0_rc1/NEWS) 에서 확인 하실 수 있습니다.

ko1님이 toruby에서 Ruby 2.1 의 신기능에 관해 발표했습니다. [All about Ruby 2.1](http://www.atdot.net/~ko1/activities/toruby05-ko1.pdf)

Konstantin Haase (@konstantinhaase) 님이 블로그에 잘 정리해 주셨습니다. [What's new in Ruby 2.1?](http://rkh.im/ruby-2.1) (영어)

## 릴리즈 코맨트

알려진 이슈:

<https://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102>

릴리즈 스케쥴과 그 밖의 정보들은 밑의 글을 참고해주십시오.

<https://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210>
