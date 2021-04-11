# Maintainer: Andrey Alekseev <andrey.android7890@gmail.com>

pkgname=('bootsplash-theme-manjaro-space-purple')
pkgver=1.1
pkgrel=2
arch=('x86_64')
pkgdesc="Beautiful Manjaro Bootsplash with space animation"
url="https://github.com/ANDRoid7890/bootsplash-theme-manjaro-space-purple"
license=('GPL')
depends=()
optdepends=('bootsplash-systemd: for bootsplash functionality')

source=('bootsplash-packer'
	'bootsplash-manjaro-space.sh'
	'bootsplash-manjaro-space-purple.initcpio_install'
	'logo.gif'
	'spinner.gif')

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

build() {
  cd "$srcdir"
  sh ./bootsplash-manjaro-space.sh
}

package_bootsplash-theme-manjaro-space-purple() {
  pkgdesc="Beautiful Manjaro Bootsplash with space animation"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-manjaro-space-purple" "$pkgdir/usr/lib/firmware/bootsplash-themes/manjaro-space-purple/bootsplash"
  install -Dm644 "$srcdir/bootsplash-manjaro-space-purple.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-manjaro-space-purple"
}
