# Maintainer: Joao Cordeiro <jlcordeiro at gmail dot com>
# Contributor: Kovivchak Evgen <oneonfire@gmail.com>

pkgname=libsc
pkgver=3.0.0
pkgrel=1
pkgdesc="Program and a library for lossless, block-sorting data compression."
arch=('i686' 'x86_64')
license=('GPL3')
url="http://libbsc.com"
depends=('gcc-libs')
source=("http://libbsc.com/Documents/bsc-$pkgver-src.zip")
md5sums=('faf3be8e2d6112d28b269e8735680d5e')

build() {
  cd $srcdir/
  make
}   
package() {
  make PREFIX=$pkgdir/usr install || return 1
}
