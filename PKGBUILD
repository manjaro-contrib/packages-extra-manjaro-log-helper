# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgdesc='Gathers selected system logs and optionally sends them to the internet.'
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.3.2
pkgrel=1
#_commit=0827f76e87e1c1008501440b7cabeb80ff40c713
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
#source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
source=("$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
sha512sums=('530f0757e3f3ed388435ba5af8dd36780df000a8f203ddf06991294615e43b40bab86eb10acb254cbc7faf377facaa45419a049d550bb126cd44d42df4de0921')

package() {
  cd $pkgname-$pkgver
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
