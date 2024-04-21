# Maintainer: bigsaltyfishes <bigsaltyfishes@gmail.com>

pkgname=molyuuos-customizations
pkgver=1.0.0
pkgrel=2
pkgdesc="MolyuuOS customizations - This package installs various MolyuuOS-specific files"
arch=('x86_64')
url="https://github.com/MolyuuOS/molyuuos-customizations"
license=('MIT')
depends=('e2fsprogs' 'btrfs-progs' 'util-linux' 'mkinitcpio' 'sudo' 'polkit')

package() {
    depends=('molyuuctl')
    
    cp -rv "${startdir}/rootfs/"* "${pkgdir}/"
    chmod 755 "${pkgdir}/usr/bin/"*
    chmod 755 "${pkgdir}/usr/bin/steamos-polkit-helpers/"*
}

# vim:set ts=2 sw=2 et:
