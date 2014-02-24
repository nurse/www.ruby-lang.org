---
layout: news_post
title: "Ruby 2.1.0-rc1 được phát hành"
author: "nurse"
translator: "Trung Lê"
date: 2013-12-20 16:53:05 +0000
lang: vi
---

Chúng tôi hân hạnh công bố bản Ruby 2.1.0-rc1.
Xin giúp chúng tôi kiểm tra các công năng mới của Ruby 2.1 trước khi ấn bản cuối được phát
hành vào 2013-12-25!

## Các thay đổi lớn so với preview 2

* gỡ bỏ curses [#8584](https://bugs.ruby-lang.org/issues/8584)

cho các thay đổi khác, xin xem [NEWS](https://github.com/ruby/ruby/blob/v2_1_0_rc1/NEWS).

## Tải về

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

## Thay đổi từ 2.0

Các thay đổi lớn:

* VM (method cache)
* RGenGC (Xem [bài thuyết trình của ko1 tại RubyKaigi](http://rubykaigi.org/2013/talk/S73) và [tại RubyConf 2013](http://www.atdot.net/~ko1/activities/rubyconf2013-ko1_pub.pdf))
* refinements [#8481](https://bugs.ruby-lang.org/issues/8481) [#8571](https://bugs.ruby-lang.org/issues/8571)
* cú pháp thay đổi
  * Rational/Complex Literal [#8430](https://bugs.ruby-lang.org/issues/8430)
  * giá trị trả về của hàm def [#3753](https://bugs.ruby-lang.org/issues/3753)
* Bignum
  * dùng GMP [#8796](https://bugs.ruby-lang.org/issues/8796)
* String#scrub [#8414](https://bugs.ruby-lang.org/issues/8414)
* Socket.getifaddrs [#8368](https://bugs.ruby-lang.org/issues/8368)
* RDoc 4.1.0 và RubyGems 2.2.0
* "literal".freeze đã dược tối ưu hoá [#9042](https://bugs.ruby-lang.org/issues/9042)
* thêm Exception#cause [#8257](https://bugs.ruby-lang.org/issues/8257)
* cập nhật thư viện như BigDecimal, JSON, NKF, Rake, RubyGems, và RDoc
* gỡ bỏ curses [#8584](https://bugs.ruby-lang.org/issues/8584)

Xem thêm chi tiết tại: [NEWS trong Ruby repository (WIP)](https://github.com/ruby/ruby/blob/v2_1_0_rc1/NEWS).

ko1 nói về các công năng mới của Ruby 2.1 tại toruby: [Tất cả về Ruby 2.1](http://www.atdot.net/~ko1/activities/toruby05-ko1.pdf)

Konstantin Haase (@konstantinhaase) tóm tắt trên trang blog của anh: [Có gì mới trong Ruby 2.1?](http://rkh.im/ruby-2.1).

## Chú thích

Các vấn đề được biết:

<https://bugs.ruby-lang.org/projects/ruby-trunk/issues?query_id=102>

Và xem luôn lịch phát hành và các thông tin khác tại:

<https://bugs.ruby-lang.org/projects/ruby-trunk/wiki/ReleaseEngineering210>
