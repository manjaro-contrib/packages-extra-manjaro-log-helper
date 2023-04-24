# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgver=0.3.4+2+ge6bbc25
pkgrel=1
pkgdesc="Gathers selected system logs and optionally sends them to the internet."
arch=('any')
url="https://gitlab.manjaro.org/ste74/manjaro-log-helper"
license=('GPL2')
depends=('bash' 'manjaro-icons' 'xclip' 'yad')
makedepends=('git')
_commit=e6bbc250265aace02cf35c66a9de6f4d082f1db8
source=("git+https://gitlab.manjaro.org/ste74/manjaro-log-helper.git#commit=$_commit")
sha256sums=('SKIP')

pkgver() {
  cd "$srcdir/$pkgname"
  git describe --tags | sed 's/^v//;s/-/+/g'
}

package() {
  cd "$srcdir/$pkgname"
  install -Dm755 mlh -t "$pkgdir/usr/bin/"
  install -Dm644 "$pkgname.desktop" -t "$pkgdir/usr/share/applications/"
}
