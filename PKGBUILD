# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgdesc='Gathers selected system logs and optionally sends them to the internet.'
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.3.4
pkgrel=1
#_commit=0827f76e87e1c1008501440b7cabeb80ff40c713
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
#source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
source=("$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
sha512sums=('76ea3e6e6c7e4da1626f011bdc06da6f448eae1a237f4b84c5378b7c75af757ee2a7e79f2f7106163a6f56d07baeac03d6437f966dfcc7edbcb53cd0b7f940b6')

package() {
  cd $pkgname-$pkgver
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
