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
source=('.config')
md5sums=('SKIP')

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/mako/" "$pkgdir/etc/skel/.config/"
    echo "Configuration files have been copied to /etc/skel."
    echo "You may copy these files to ~/.config/ and make any changes you wish."
}
