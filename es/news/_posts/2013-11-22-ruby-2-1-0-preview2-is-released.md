---
layout: news_post
title: "Liberado Ruby 2.1.0-preview2"
author: "nurse"
translator: "David Padilla"
date: 2013-11-22 22:00:00 +0000
lang: es
---

Nos complace anunciar la entrega de Ruby 2.1.0-preview2.
Por favor ayudanos a probar las nuevas características de Ruby 2.1 antes de
la entrega final.

## Cambios notables desde preview 1

* Corrección [Desborbamiento de pila en el interprete de flotantes (CVE-2013-4164)](https://www.ruby-lang.org/es/news/2013/11/22/heap-overflow-in-floating-point-parsing-cve-2013-4164/)
* "literal".freeze ha sido optimizado [#9042](https://bugs.ruby-lang.org/issues/9042)
* Remover el sufijo f de el literal de cadena [#9042](https://bugs.ruby-lang.org/issues/9042)
* Corregir un problema de consumo de memoria en RGenGC ([r43532](http://svn.ruby-lang.org/cgi-bin/viewvc.cgi?view=rev&revision=43532) y [r43755](http://svn.ruby-lang.org/cgi-bin/viewvc.cgi?view=rev&revision=43755))
* Agregar Exception#cause [#8257](https://bugs.ruby-lang.org/issues/8257)
* Actualizar librerías como json, nkf, rake, RubyGems, and RDoc.

## Descarga

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

## Cambios desde 2.0

Los cambios mas notables son:

* VM (cache de métodos)
* RGenGC (Ver la [presentación en RubyKaigi](http://rubykaigi.org/2013/talk/S73) y [RubyConf 2013](http://www.atdot.net/~ko1/activities/rubyconf2013-ko1_pub.pdf) de ko1)
* Refinements [#8481](https://bugs.ruby-lang.org/issues/8481) [#8571](https://bugs.ruby-lang.org/issues/8571)
* Cambios en la sintáxis
  * Literales de Rational/Complex [#8430](https://bugs.ruby-lang.org/issues/8430)
  * el valor de retorno de def [#3753](https://bugs.ruby-lang.org/issues/3753)
* Bignum
  * Uso de enteros de 128bit [#8509](https://bugs.ruby-lang.org/issues/8509)
  * Uso de GMP [#8796](https://bugs.ruby-lang.org/issues/8796)
* String#scrub [#8414](https://bugs.ruby-lang.org/issues/8414)
* Socket.getifaddrs [#8368](https://bugs.ruby-lang.org/issues/8368)
* RDoc 4.1.0.preview.2 y RubyGems 2.2.0.preview.2

Ver detalles de los cambios:
[NOTICIAS en el repositorio de Ruby (WIP)](https://github.com/ruby/ruby/blob/v2_1_0_preview2/NEWS).

ko1 habló acerca de las nuevas características de Ruby 2.1 en
toruby: [Todo acerca de Ruby 2.1](http://www.atdot.net/~ko1/activities/toruby05-ko1.pdf)

Konstantin Haase (@konstantinhaase) escribió un excelente resumen de los
cambios en su blog post: [What's new in Ruby 2.1?](http://rkh.im/ruby-2.1).

## Comentarios

Problemas conocidos:

[http://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102](http://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102)

Ver también la agenda de entregas y otra información:

[http://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210](http://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210)

