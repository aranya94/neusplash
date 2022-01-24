# Maintainer: Aranya Das <aranyadas@hotmail.com>
pkgname=neusplash
_destname1="/usr/share/plasma/look-and-feel"
_destname2="/etc"
_destname3="/etc"
_destname4="/etc"
pkgver=21.08
pkgrel=6
pkgdesc="Custom Splash for TDLinux"
arch=('any')
url="https://github.com/aranya94"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	plasmapkg2 -u ${pkgdir}/usr/share/plasma/look-and-feel/org.kde.neusplash.desktop
}

