# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgdesc='Gathers selected system logs and optionally sends them to the internet.'
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.3
pkgrel=1
#_commit=93134c25ee4036e1562af4019a3ef0f055a29aab
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
#source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
source=("$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
sha512sums=('7ed8da1306e3cf4c888d98d5b1fe7c94f5d4b2e84c82fbfdca2ec5d56de114fbda5bf904497f63e468d78e40eb1e5b097ae7298efd133674f944828eb832ab1b')

package() {
  cd $pkgname-$pkgver
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
