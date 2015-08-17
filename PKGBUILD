# Maintainer: Daniel Wallace <danielwallace at gtmanfred dot com>
pkgname=python2-pyxenstore
pkgver=0.0.2
pkgrel=2
pkgdesc="Python XenStore Module"
arch=('x86_64' 'i686')
url="https://pypi.python.org/pypi/pyxenstore"
license=('GPL')
depends=('python2' 'xenstore')
makedepends=('python2-distribute')
source=("https://pypi.python.org/packages/source/p/${pkgname#*-}/${pkgname#*-}-$pkgver.tar.gz")
md5sums=('4da2524ed0ec9439afc5c9a46ac21c6c')

build() {
  cd "$srcdir/${pkgname#*-}-$pkgver"
  python2 setup.py build
}
package() {
  cd "$srcdir/${pkgname#*-}-$pkgver"
  python2 setup.py install --root="$pkgdir/"
}

# vim:set ts=2 sw=2 et:
