# Maintainer: William Penton <william@nexxuz.co>

pkgname=gitkraken-cli
pkgver=3.1.1
pkgrel=2
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
sha256sums=('c43456aafc0e5d12808ef19b9a8aba2e76b59bf7b3bb2ecc846be75458600686')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk_"$pkgver"_linux_amd64/gk "$pkgdir"/usr/local/bin/
}
