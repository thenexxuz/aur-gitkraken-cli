# Maintainer: William Penton <william@nexxuz.co>

pkgname=gitkraken-cli
pkgver=3.1.9
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
sha256sums=('73077548d534b3239046a9ebc9cb2eef0d33f12bdba3e3ca1e6fb6b113995964')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk "$pkgdir"/usr/local/bin/
}
