# Maintainer: Shantanu R <shantanu@ramanujapuram.com>

pkgname=rofi-firefox-profiles
pkgver=1.1.1
pkgrel=3
pkgdesc="Launch your default browser (firefox, zen, brave) with a selected profile using your default or custom rofi config"
arch=('any')
url="https://github.com/shanten/rofi-firefox-profiles"
license=('MIT')
depends=('python' 'rofi')
optdepends=('firefox: optional if using firefox explicitly'
            'zen-browser: optional if using zen explicitly' 
            'brave: optional if using brave explicitly'
           )
source=(
  "$pkgname"
  "config.ini"
)
sha256sums=('SKIP' 'SKIP')

package() {
    install -Dm755 "$srcdir/$pkgname" "$pkgdir/usr/bin/$pkgname"
    install -Dm644 "$srcdir/config.ini" "$pkgdir/etc/$pkgname/config.ini"
}
