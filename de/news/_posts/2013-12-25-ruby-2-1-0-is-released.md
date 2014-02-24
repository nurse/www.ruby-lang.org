---
layout: news_post
title: "Ruby 2.1.0 veröffentlicht"
author: "nurse"
translator: "Quintus"
date: 2013-12-25 16:00:00 +0000
lang: de
---

Wir freuen uns, die Veröffentlichung von Ruby 2.1.0 ankündigen zu können.

Ruby 2.1 bietet zahlreiche Verbesserungen, darunter
Geschwindigkeitsvorteile ohne größere Inkompatibilitäten.

Versuchen Sie es!

## Download

* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.tar.bz2](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.tar.bz2)
  * SIZE:   12007442 bytes
  * MD5:    1546eeb763ac7754365664be763a1e8f
  * SHA256: 1d3f4ad5f619ec15229206b6667586dcec7cc986672c8fbb8558161ecf07e277
* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.tar.gz](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.tar.gz)
  * SIZE:   15076389 bytes
  * MD5:    9e6386d53f5200a3e7069107405b93f7
  * SHA256: 3538ec1f6af96ed9deb04e0965274528162726cc9ba3625dcf23648df872d09d
* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.zip](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0.zip)
  * SIZE:   16603067 bytes
  * MD5:    2fc3a80b56da81b906a9bb6fc7ca8399
  * SHA256: d40d7bfb39ca2e462dea61dcbbcf33426b60e6e553335c3afb39b4d827a6891c

## Änderungen seit 2.0

Die aufälligsten Änderungen sind:

* VM (Methodencache)
* RGenGC (Siehe ko1s
  [RubyKaigi-Präsentation](http://rubykaigi.org/2013/talk/S73) und
  [RubyConf-2013-Präsentation](http://www.atdot.net/~ko1/activities/rubyconf2013-ko1_pub.pdf)
* Refinements [#8481](https://bugs.ruby-lang.org/issues/8481) [#8571](https://bugs.ruby-lang.org/issues/8571)
* Syntaxänderungen
  * Rational/Complex-Literal
    [#8430](https://bugs.ruby-lang.org/issues/8430)
  * Rückgabewert von `def` [#3753](https://bugs.ruby-lang.org/issues/3753)
* Bignum
  * Verwende GMP [#8796](https://bugs.ruby-lang.org/issues/8796)
* String#scrub [#8414](https://bugs.ruby-lang.org/issues/8414)
* Socket.getifaddrs [#8368](https://bugs.ruby-lang.org/issues/8368)
* RDoc 4.1.0 und RubyGems 2.2.0
* `"literal".freeze` wurde optimiert [#9042](https://bugs.ruby-lang.org/issues/9042)
* Exception#cause hinzugefügt [#8257](https://bugs.ruby-lang.org/issues/8257)
* Bibliotheken wie BigDecimal, JSON, NKF, Rake, RubyGems und RDoc aktualisiert
* Curses entfernt [#8584](https://bugs.ruby-lang.org/issues/8584)

Siehe die Datei [NEWS im
Ruby-Repository](https://github.com/ruby/ruby/blob/v2_1_0/NEWS) für
weitere Informationen.
