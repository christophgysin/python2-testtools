# Maintainer: Neil Santos <nsantos16+aur@gmail.com>

pkgname=python2-testtools
_pkgname=${pkgname#*-}
pkgver=0.9.39
pkgrel=1
pkgdesc='Extensions to the Python standard library unit testing framework'
arch=('i686' 'x86_64')
url='https://github.com/testing-cabal/testtools'
license=('GPL')
depends=('python2')
provides=("python-testtools=${pkgver}")
source=(http://pypi.python.org/packages/source/${_pkgname:0:1}/${_pkgname}/${_pkgname}-${pkgver}.tar.gz)
md5sums=('a604dfd54cc5f06599c24aa4c26a3126')


build() {
    cd ${srcdir}/${_pkgname}-${pkgver}
    python2 setup.py build
}

package() {
    cd ${srcdir}/${_pkgname}-${pkgver}
    python2 setup.py install \
        --skip-build \
        --optimize=1 \
        --prefix=/usr \
        --root=${pkgdir}
}
