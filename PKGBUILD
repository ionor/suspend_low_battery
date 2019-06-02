# Maintainer: Johan Noren
pkgname=suspend_low_battery
arch=('x86_64')
pkgver=1
pkgrel=2
pkgdesc="Small script that checks for battery status and suspends when critical"
license=('GPL')
source=("suspend_low_battery" "suspend_low_battery.service" "config")

package() {
	cd "${srcdir}/"
    install -Dm0755 suspend_low_battery "${pkgdir}/usr/bin/suspend_low_battery"
    install -Dm0644 suspend_low_battery.service "${pkgdir}/etc/systemd/system/suspend_low_battery.service"
    install -Dm0644 config "${pkgdir}/etc/xdg/suspend_low_battery/config"
}

md5sums=('23426ac7be74579055b05661c70098af'
         'd503a121130230c2365ee9b917eae1b0'
         '9db3840a7e893e3cf67c8d30f01c8c07')
