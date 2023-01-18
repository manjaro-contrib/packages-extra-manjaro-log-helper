# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgdesc='Gathers selected system logs and optionally sends them to the internet.'
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.3.3
pkgrel=1
#_commit=0827f76e87e1c1008501440b7cabeb80ff40c713
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
#source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
source=("$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
sha512sums=('bb761472e1e367796d83bf566da2ecda6f1111347e66638d9f23535198368d5456bfd58cae27a526b36a6e9a06977664a5de85d4056cb3c7c8a5e64184d3997e')

package() {
  cd $pkgname-$pkgver
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
