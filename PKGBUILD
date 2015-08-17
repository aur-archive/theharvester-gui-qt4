# Maintainer: Joshua Strot <joshuastrot@mail.com>

pkgname=theharvester-gui-qt4
_pkgname=theHarvester-gui
pkgver=0.9.1
pkgrel=1
pkgdesc="QT frontend for theHarvester in QT4."
url="https://github.com/dcell/$_pkgname"
arch=('i686' 'x86_64')
license=('GPL2')
makedepends=('git')
depends=('theharvester-git' 'python2' 'python2-pyqt4' 'pyqt4-common' 'qt4')
provides=('theharvester-gui')
conflicts=('theharvester-gui')
source=("git://github.com/dcell/$_pkgname.git")
sha1sums=('SKIP')

package() {
    cd "$srcdir/$_pkgname"
    
    git checkout tags/v$pkgver 2> /dev/null

    ./install.sh -d $pkgdir -v qt4
}
