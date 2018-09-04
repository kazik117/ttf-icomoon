# Maintainer: Mateusz Kazmierczak <kazik117@gmail.com> PGP-Key: C0DEA350

pkgname=ttf-icomoon
epoch=1
pkgver=1.0
pkgrel=2
pkgdesc='Custom icon font. Icomoon'
arch=('any')
license=('Unknown')
url="http://mkazik.pl"
depends=('fontconfig' 'xorg-fonts-encodings' 'xorg-font-utils')
makedepends=('unzip')
install=$pkgname.install
#noextract=("icomoon-${pkgver}-${pkgrel}.zip")
source=(
  "icomoon-${pkgver}-${pkgrel}.zip"
)
package()
{
  #bsdtar is not working
  cd $srcdir
  unzip -qqo icomoon-${pkgver}-${pkgrel}.zip

  install -d $pkgdir/usr/share/fonts/TTF/ 
  install -m644 $srcdir/fonts/*.ttf $pkgdir/usr/share/fonts/TTF/ 
}

sha1sums=('9697ab039a57ed418a7296c51e49f19bf13605f5')
