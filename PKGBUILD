# Maintainer: Markus Pesch <markus.pesch@cryptic.systems>

pkgname=mint-backgrounds-nadia
pkgver=1.4
pkgrel=1
pkgdesc="The backgrounds included in Linux Mint 14 Nadia"
license=('Various')
arch=('any')
url="http://packages.linuxmint.com/pool/main/m/${pkgname}"
source=("${url}/${pkgname}_$pkgver.tar.gz")
sha256sums=('fa081c3ae4e909e372c41b0119c5c5a4b7beabaf05299ec1d47190dbf1368d0d')

package() {
	mkdir --parents ${pkgdir}/usr/share/backgrounds/linuxmint-nadia
	mkdir --parents ${pkgdir}/usr/share/{cinnamon-background-properties,gnome-background-properties}

  cp --archive ${srcdir}/${pkgname}/usr/share/backgrounds/linuxmint-nadia ${pkgdir}/usr/share/backgrounds
	cp --archive ${srcdir}/${pkgname}/usr/share/gnome-background-properties/* ${pkgdir}/usr/share/cinnamon-background-properties
	cp --archive ${srcdir}/${pkgname}/usr/share/gnome-background-properties/* ${pkgdir}/usr/share/gnome-background-properties
}