# Maintainer: Your Name <admin@matsyos.ml>
pkgname=matsya-icons
pkgver=0.8
pkgrel=1
pkgdesc="System default icon theme of Matsya_Os"
arch=('any')
url="https://github.com/matsyaos/icons"
license=('GPL')
groups=('cutefish')
depends=()
makedepends=('extra-cmake-modules' 'ninja')
source=('git'+'https://github.com/matsyaos/icons')
md5sums=('SKIP')

build() {
  cd icons-$pkgver

  cmake -GNinja -DCMAKE_INSTALL_PREFIX=/usr .
  ninja
}

package() {
  cd icons-$pkgver
  DESTDIR="$pkgdir" ninja install
}
