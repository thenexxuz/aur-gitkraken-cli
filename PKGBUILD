# Maintainer: William Penton <william@nexxuz.co>

pkgname=gitkraken-cli
pkgver=3.1.5
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
sha256sums=('ff2bc293f66030125205b203e44f48f78f62ec996d6e567489aa631a4aa39897')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk_"$pkgver"_linux_amd64/gk "$pkgdir"/usr/local/bin/
}
