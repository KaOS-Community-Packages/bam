pkgname=bam
pkgver=0.4.0
pkgrel=1
pkgdesc="A fast and flexible build system using Lua"
arch=('x86_64')
url="http://github.com/matricks/bam"
license=('ZLIB')
source=("http://github.com/downloads/matricks/bam/bam-${pkgver}.tar.gz")
md5sums=('2f8e8336b8884110e8a355b12c9fa58a')

build() {
	cd ${srcdir}/${pkgname}-${pkgver}
	sh make_unix.sh
}

package() {
	cd ${srcdir}/${pkgname}-${pkgver}
	install -Dm755 bam ${pkgdir}/usr/bin/bam
}
