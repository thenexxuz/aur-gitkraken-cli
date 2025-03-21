# Maintainer: William Penton <william@penton.us>

pkgname=gitkraken-cli
pkgver=3.0.0
pkgrel=1
pkgdesc="The intuitive, fast, and beautiful cross-platform Git client."
url="https://www.gitkraken.com/"
provides=('gk-cli')
arch=('x86_64')
license=('custom')
optdepends=('git-lfs: git-lfs support'
            'org.freedesktop.secrets: Provides ways to store passwords and encryption keys')
makedepends=()
backup=()
install=''
source=(
    "${pkgname}-${pkgver}-beta.zip::https://github.com/gitkraken/gk-cli/releases/download/v${pkgver}-beta/gk_${pkgver}-beta_linux_amd64.zip"
)
sha256sums=('45eb6796c9ef521bfaf61f4496341077d09a13a662cb5d9bf05b1815b6f53930')

package() {
    install -d "$pkgdir"/usr/local/bin
    cp -R "$srcdir"/gk_3.0.0-beta_linux_amd64/gk "$pkgdir"/usr/local/bin/
}
