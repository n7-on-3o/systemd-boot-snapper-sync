# Maintainer: n7-on-3o <fanton.io@icloud.com>
pkgname=systemd-boot-snapper-tools-git
_pkgname=systemd-boot-snapper-tools
pkgver=1.0.0
pkgrel=1
pkgdesc="Automated systemd-boot management and rollback tools for Snapper"
arch=('any')
url="https://github.com/youruser/systemd-boot-snapper-tools"
license=('GPL')
depends=('snapper' 'btrfs-progs' 'binutils' 'util-linux' 'sed')
makedepends=('git')
provides=("$_pkgname")
conflicts=("$_pkgname")
source=("git+${url}")
md5sums=('SKIP')

package() {
  cd "$srcdir/$_pkgname"
  make DESTDIR="$pkgdir" PREFIX=/usr install
}
