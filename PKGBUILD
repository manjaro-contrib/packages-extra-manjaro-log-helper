# Maintainer: Stefano Capitani <stefano@manjaro.org>

pkgname=manjaro-log-helper
pkgver=0.3.4+1+g1f6efe9
pkgrel=1
pkgdesc="Gathers selected system logs and optionally sends them to the internet."
arch=('any')
url="https://gitlab.manjaro.org/ste74/manjaro-log-helper"
license=('GPL2')
depends=('bash' 'manjaro-icons' 'wgetpaste' 'xclip' 'yad')
makedepends=('git')
_commit=1f6efe95615c1bbec77e696f25fc481fd0178880
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
