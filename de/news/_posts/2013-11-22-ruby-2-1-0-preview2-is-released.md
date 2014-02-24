---
layout: news_post
title: "Ruby 2.1.0-preview2 veröffentlicht"
author: "nurse"
translator: "Quintus"
date: 2013-11-22 22:00:00 +0000
lang: de
---

Wir freuen uns, die Veröffentlichung von Ruby 2.1.0-preview2
ankündigen zu können. Bitte testen Sie die neuen Features von Ruby 2.1
vor dem finalen Release!

## Wesentliche Änderungen seit preview1

* Korrigiere [Heap-Überlauf beim Parsen von Floating-Point (CVE-2013-4164)](https://www.ruby-lang.org/de/news/2013/11/22/heap-overflow-in-floating-point-parsing-cve-2013-4164/)
* `"literal".freeze` wurde optimiert [#9042](https://bugs.ruby-lang.org/issues/9042)
* `f`-Suffix von String-Literalen entfernt [#9024](https://bugs.ruby-lang.org/issues/9042)
* Korrigiere Speicherproblem im RGenGC ([r43532](http://svn.ruby-lang.org/cgi-bin/viewvc.cgi?view=rev&revision=43532) und [r43755](http://svn.ruby-lang.org/cgi-bin/viewvc.cgi?view=rev&revision=43755))
* Füge Exception#cause hinzu [#8257](https://bugs.ruby-lang.org/issues/8257)
* Aktualisiere Programmbibliotheken wie json, nkf, rake, RubyGems und RDoc.

## Download

* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.tar.bz2](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.tar.bz2)

      SIZE:   11432454 bytes
      MD5:    9d566a9b2d2e7e35ad6125e2a14ce672
      SHA256: 780fddf0e3c8a219057d578e83367ecfac5e945054b9f132b3b93ded4802d1ce

* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.tar.gz](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.tar.gz)

      SIZE:   14416029 bytes
      MD5:    ba2b95d174e156b417a4d580a452eaf5
      SHA256: a9b1dbc16090ddff8f6c6adbc1fd0473bcae8c69143cecabe65d55f95f6dbbfb

* [http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.zip](http://cache.ruby-lang.org/pub/ruby/2.1/ruby-2.1.0-preview2.zip)

      SIZE:   16110720 bytes
      MD5:    2ad1aa3d89ae32607cf14fc73b192de1
      SHA256: cc2f7f8e05daed716489e5480e6365a711a13ed7747dbc59e989a41fe2805076

## Änderungen seit 2.0

Die auffälligsten Änderungen sind:

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
  * Verwende 128bit-Integers [#8509](https://bugs.ruby-lang.org/issues/8509)
  * Verwende GMP [#8796](https://bugs.ruby-lang.org/issues/8796)
* String#scrub [#8414](https://bugs.ruby-lang.org/issues/8414)
* Socket.getifaddrs [#8368](https://bugs.ruby-lang.org/issues/8368)
* RDoc 4.1.0.preview.2 und RubyGems 2.2.0.preview.2


Für weitere Details, siehe [NEWS im Ruby-Repository (WIP)](https://github.com/ruby/ruby/blob/v2_1_0_preview2/NEWS).

ko1 sprach auf der _toruby_ über die neuen Features von Ruby 2.1:
[Alles über Ruby 2.1](http://www.atdot.net/~ko1/activities/toruby05-ko1.pdf).

Konstantin Haase (@konstantinhaase) hat auf seinem Blog eine gute
Zusammenfassung veröffentlicht: [Was ist neu in Ruby 2.1?](http://rkh.im/ruby-2.1)

## Veröffentlichungskommentar

Bekannte Probleme sind:

[http://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102](http://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102)

Siehe auch den Veröffentlichungszeitplan für weitere Informationen:

[http://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210](http://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210)
