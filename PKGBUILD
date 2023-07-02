# Maintainer: Redson <redson at riseup.net>
# Thanks for chaotic-aur's package that I've used as template!

pkgname='archwin-keyring'
pkgver='20230702'
pkgrel=1
pkgdesc='ArchWin PGP keyring'
arch=('any')
url='https://archwin.github.io/repo/'
license=('GPL')
depends=('archlinux-keyring')
install=$pkgname.install
source=("keyring-$pkgver-$pkgrel.tar.gz::https://github.com/archwin/keyring/archive/$pkgver-$pkgrel.tar.gz")
sha512sums=('af982cee51b743fb79a539bf5a025ef3422845b187e49d9256664522cb3f3066ee97dd891abffbe9b5ed112256dda079358c11d7053899b32cc9f0f79b171f5c')

package() {
  cd "$srcdir/keyring-$pkgver-$pkgrel"
  make PREFIX=/usr "DESTDIR=$pkgdir" install
}

