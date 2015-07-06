pkgname=ctris
pkgver=0.42
pkgrel=1
pkgdesc='Console based Tetris clone'
arch=('i686' 'x86_64')
url='http://www.hackl.dhs.org/ctris/'
license=('GPL2')
depends=('ncurses' 'guile')
source=("${pkgname}-${pkgver}.tar.bz2")
sha1sums=('f367f4b91724f9c272f2e7bf4523721a8f3c1f99')

build() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make
}

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make DESTDIR="${pkgdir}" install
}
