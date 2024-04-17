# Maintainer: bigsaltyfishes <bigsaltyfishes@gmail.com>

pkgname=molyuuos-customizations
pkgver=r1.3428ae6
pkgrel=1
branch="main"
pkgdesc="MolyuuOS customizations - This package installs various MolyuuOS-specific files"
arch=('x86_64')
url="https://github.com/MolyuuOS/molyuuos-customizations"
license=('MIT')
depends=('e2fsprogs' 'btrfs-progs' 'util-linux' 'mkinitcpio' 'molyuuctl' 'sudo' 'polkit')

pkgver() {
# Git, no tags available
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cp -rv "${startdir}/rootfs/"* "${pkgdir}/"
    chmod 755 "${pkgdir}/usr/bin/"*
    chmod 755 "${pkgdir}/usr/bin/steamos-polkit-helpers/"*
}

# vim:set ts=2 sw=2 et:
