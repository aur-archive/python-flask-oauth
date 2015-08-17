pkgname=python-flask-oauth
_pkgname=Flask-OAuth
pkgver=0.12
pkgrel=1
pkgdesc='Adds OAuth support to Flask (python3 version)'
arch=('i686', 'x86_64')
url='https://pypi.python.org/pypi/Flask-OAuth'
license=('BSD')
depends=('python-oauth2' 'python-flask')
source=("https://pypi.python.org/packages/source/F/${_pkgname}/${_pkgname}-${pkgver}.tar.gz")
md5sums=('eea1295eb191f3d3064c61df5a10cdc1')

build() {
    cd "$srcdir/${_pkgname}-${pkgver}"

    python setup.py build
}

package() {
    cd "$srcdir/${_pkgname}-${pkgver}"

    python setup.py install --root=${pkgdir} --optimize=1
}
