# Maintainer: William Penton <william@nexxuz.co>

pkgname=gitkraken-cli
pkgver=3.1.10
pkgrel=1
pkgdesc="The intuitive, fast, and beautiful cross-platform Git client."
url="https://www.gitkraken.com/"
provides=('gitkraken')
arch=('x86_64')
license=('custom')
optdepends=('git-lfs: git-lfs support'
            'org.freedesktop.secrets: Provides ways to store passwords and encryption keys')
makedepends=()
backup=()
install=''
source=(
    "${pkgname}-${pkgver}.zip::https://github.com/gitkraken/gk-cli/releases/download/v${pkgver}/gk_${pkgver}_linux_amd64.zip"
)
sha256sums=('4f55a8a12032340de507f618c4688de066fe8b30aec96c13b2bd45697340722f')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk "$pkgdir"/usr/local/bin/
}
