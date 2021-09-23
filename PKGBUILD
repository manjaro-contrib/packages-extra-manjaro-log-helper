# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgdesc='Gathers selected system logs and optionally sends them to the internet.'
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.3.1
pkgrel=1
#_commit=0827f76e87e1c1008501440b7cabeb80ff40c713
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
#source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
source=("$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
sha512sums=('aaa4549b40271612f6e7f60806e20ddbc327ea9f8206ce063b0cbb12ab25304edb78a6d2a3a88b399725f2666e43062a50ec6036280fbcf540872157836fcdbd')

package() {
  cd $pkgname-$pkgver
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
