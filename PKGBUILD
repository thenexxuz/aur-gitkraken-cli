# Maintainer: William Penton <william@nexxuz.co>

pkgname=gitkraken-cli
pkgver=3.1.32
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
sha256sums=('c8dc699abdc3a5098113cc12092544811e025983c7ac8dcd066e06b41c6851b8')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk "$pkgdir"/usr/local/bin/
}
