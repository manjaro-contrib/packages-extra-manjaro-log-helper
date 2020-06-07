# Maintainer: Stefano Capitani <stefano@manjaro.org>
 
pkgname=manjaro-log-helper
pkgdesc="Gathers selected system logs and optionally sends them to the internet."
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.2
pkgrel=1
_commit=93134c25ee4036e1562af4019a3ef0f055a29aab
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons' 'yad')
source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
sha512sums=('9959ad3a7315a03c4e199fbe75886fece22ab2ad8b3c35b0c048bc48c0a09c098b3b87d995854fde498ae9a1b52d9ff816a7a7515e1cc6bd6617e6fcfd2897c2')

package() {
  cd $pkgname-$_commit
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm755 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
