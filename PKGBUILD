pkgname=2gis-biysk
pkgver=55
pkgrel=2
pkgdesc="Map of Biysk for 2GIS, May 2013"
arch=('i686' 'x86_64')
url="http://biysk.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Biysk-55.orig.zip")
md5sums=('c4699463b9c11d20037267fd6dfec703')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Biysk.dgdat" "${pkgdir}/opt/2gis/biysk.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Biysk.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/biysk.dglf" || return 1
}
