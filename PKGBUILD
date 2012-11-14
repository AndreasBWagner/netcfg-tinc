# Maintainer: Florian Kellmer <florian.kellmer@linuxmail.org>
pkgname=netcfg-tinc
pkgver=0.1
pkgrel=1
pkgdesc="Tinc support for netcfg"
arch=(i686 x86_64)
url="https://github.com/floyd2/netcfg-tinc"
license=('MIT')
depends=('netcfg' 'tinc')
source=(tinc.example tinc)
md5sums=('ce771990c1f1ffa3ceba4ec503cded3d'
         'b91a3358605c3b0adf73244ef34a2cc2')

build() {
  install -Dm644 $srcdir/tinc.example $pkgdir/etc/network.d/examples/tinc
  install -Dm755 $srcdir/tinc $pkgdir/usr/lib/network/connections/tinc
}
