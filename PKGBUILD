# $Id: PKGBUILD 55474 2011-09-13 01:29:57Z ebelanger $
# Contributor: Roman Kyrylych <Roman.Kyrylych@gmail.com>
# Contributor: Dario Andres Rodriguez <darzephyr@gmail.com>
# Maintainer: Daniel J Griffiths <ghost1227@archlinux.us>

pkgname=xcursor-jimmac
pkgver=2.0
pkgrel=6
pkgdesc="Jimmac (Jimmac0) cursor theme"
arch=('any')
url="http://www.kde-look.org/content/show.php?content=28281"
license=('GPL')
conflicts=('jimmac')
replaces=('jimmac')
source=(http://www.kde-look.org/CONTENT/content-files/28281-Jimmac0.tar.bz2 \
        http://www.kde-look.org/CONTENT/content-files/6550-Jimmac.tar.gz index.theme)
md5sums=('6fe7d2f7d6b28e8e2de98cb6125f84fa'
         '46fb39d5e176dfc3bfa2c65743301f03'
         '58ea5ca96b219f649089de2044fd5998')

package() {
	mkdir -p "${pkgdir}"/usr/share/icons/Jimmac/
	cp -R "${srcdir}"/Jimmac/jimmac/cursors \
		"${pkgdir}"/usr/share/icons/Jimmac/cursors
	cp "${srcdir}"/Jimmac0/cursors/plus \
		"${pkgdir}"/usr/share/icons/Jimmac/cursors
	cp "${srcdir}"/Jimmac0/cursors/question_arrow \
		"${pkgdir}"/usr/share/icons/Jimmac/cursors
	install -Dm644 "${srcdir}"/index.theme \
		"${pkgdir}"/usr/share/icons/Jimmac/index.theme
}
