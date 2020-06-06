# Maintainer: Stefano Capitani <stefano@manjaro.org>
 
pkgname=manjaro-log-helper
pkgdesc="Gathers selected system logs and optionally sends them to the internet."
url=https://gitlab.manjaro.org/ste74/manjaro-log-helper
pkgver=0.1
pkgrel=1
_commit=2586a7dc1008e5291ebdad645f8210012c45ea82
arch=('any')
license=('GPL2')
depends=('bash' 'pastebinit' 'xclip' 'manjaro-icons')
source=("$pkgname-$_commit.tar.gz::$url/-/archive/$_commit/$pkgname-$_commit.tar.gz")
sha512sums=('c693a57c15e8a8e3d7304272f7b07d84c3b6c976bfa18a748d14f21b7fcba2399f227b50173c0f3c7419d1a9ac5d0a5719e82c744b6308511a62649bfa8452e7')

package() {
  cd $pkgname-$_commit
  install -Dm755 mlh $pkgdir/usr/bin/mlh

  install -d $pkgdir/usr/share/applications
  install -Dm755 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
