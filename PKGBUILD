# Maintainer: grmat <grmat@sub.red>

pkgname=amdgpu-fancontrol
pkgdesc="amdgpu-fancontrol"
pkgver=1.0
pkgrel=1
arch=('any')
license=('GPL')
depends=('systemd' 'bc')

source=('amdgpu-fancontrol' 'amdgpu-fancontrol.service')
sha256sums=('5639b219bbef619d1314179903a6f8583dfbb2d9d43a88424f344f3f5c2545f6'
            '509d5c2676ea0aa23918bebd1b4f5f0268b0a6a68a27650ce487dfb58f27e70c')

package() {
    mkdir -p ${pkgdir}/usr/bin
    cp ${srcdir}/amdgpu-fancontrol ${pkgdir}/usr/bin/
    mkdir -p ${pkgdir}/usr/lib/systemd/system
    cp ${srcdir}/amdgpu-fancontrol.service ${pkgdir}/usr/lib/systemd/system/
}
