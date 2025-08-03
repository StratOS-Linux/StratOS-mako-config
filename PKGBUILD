# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-mako-config
pkgver=1.0
pkgrel=1
pkgdesc="Mako configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'mako'
)
install=stratos-mako-config.install
source=('.config')
md5sums=('SKIP')
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/mako/" "$pkgdir/etc/skel/.config/"
}
