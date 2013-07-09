# $Id: PKGBUILD 60970 2011-12-19 21:33:58Z spupykin $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Dag Odenhall <dag.odenhall@gmail.com>
# Contributor: Grigorios Bouzakis <grbzks@gmail.com>

pkgname=dwm
pkgver=6.0
pkgrel=1
pkgdesc="A dynamic window manager for X"
url="http://dwm.suckless.org"
arch=('i686' 'x86_64')
license=('MIT')
options=(zipman)
depends=('libx11' 'libxinerama')
install=dwm.install
source=(http://dl.suckless.org/dwm/dwm-$pkgver.tar.gz
	config.h
	dwm.desktop)
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2453e037f46449774ec8afab49b4f1a2'
         '939f403a71b6e85261d09fc3412269ee')

build() {
  cd $srcdir/$pkgname-$pkgver
  cp $srcdir/config.h config.h
  sed -i 's/CPPFLAGS =/CPPFLAGS +=/g' config.mk
  sed -i 's/^CFLAGS = -g/#CFLAGS += -g/g' config.mk
  sed -i 's/^#CFLAGS = -std/CFLAGS += -std/g' config.mk
  sed -i 's/^LDFLAGS = -g/#LDFLAGS += -g/g' config.mk
  sed -i 's/^#LDFLAGS = -s/LDFLAGS += -s/g' config.mk
  make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11
}

package() {
  cd $srcdir/$pkgname-$pkgver
  make PREFIX=/usr DESTDIR=$pkgdir install
  install -m644 -D LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE
  install -m644 -D README $pkgdir/usr/share/doc/$pkgname/README
  install -m644 -D $srcdir/dwm.desktop $pkgdir/usr/share/xsessions/dwm.desktop
}
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '6a34aa1de37c344bbfb675f91427e497'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '601090328dac84a9d3ef849f91d991ff'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '43684e6ed8f698328c5995663a0b3a8e'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'da93725eb674f25fcd4b9158c6dc8eee'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '63f8cede666353c0a835400fce8ad833'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'da93725eb674f25fcd4b9158c6dc8eee'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '63f8cede666353c0a835400fce8ad833'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'ebdf2f9ba79ef09ef47515b263c54c0b'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'd0d18ef166903815aeab9a29cd293cf0'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '001552fc5f6fe9a86117e78e25e33c62'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '1abfc815bd7a8b1c49fc40f1eea50f3b'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '95c338a410cdfc6bb1eb6605de5ce19f'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '46377fa0c7c74d821f22a090c090427e'
         '939f403a71b6e85261d09fc3412269ee')
