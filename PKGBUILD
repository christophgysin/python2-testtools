# Maintainer: Neil Santos <nsantos16+aur@gmail.com>

pkgname=python2-testtools
pkgver=0.9.35
pkgrel=1
pkgdesc='Extensions to the Python standard library unit testing framework'
arch=('i686' 'x86_64')
url='https://launchpad.net/testtools'
license=('GPL')
depends=('python2')
provides=("python-testtools=${pkgver}")
source=("http://pypi.python.org/packages/source/t/testtools/testtools-$pkgver.tar.gz")
md5sums=('a604dfd54cc5f06599c24aa4c26a3126')

build() {
  cd "$srcdir/testtools-$pkgver"
  python2 setup.py install --prefix=/usr --root="$pkgdir" || return 1
}
