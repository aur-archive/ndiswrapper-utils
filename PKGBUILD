# Maintainer: Tobias Powalowski <tpowa@archlinux.org>

pkgname=ndiswrapper-utils
pkgver=1.56
pkgrel=2
pkgdesc="Binaries for ndiswrapper module"
arch=('i686' 'x86_64')
license=('GPL')
url="http://ndiswrapper.sourceforge.net"
depends=('wireless_tools' 'glibc' 'perl')
replaces=('ndiswrapper-bin')
conflicts=('ndiswrapper-bin')
source=(http://downloads.sourceforge.net/ndiswrapper/ndiswrapper-$pkgver.tar.gz)
md5sums=('1431f7ed5f8e92e752d330bbb3aed333')

build() {
  cd $srcdir/ndiswrapper-$pkgver/utils
  make
}

package() {
  cd $srcdir/ndiswrapper-$pkgver/utils
  make DESTDIR=$pkgdir install
}
