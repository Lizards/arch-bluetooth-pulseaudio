pkgbase=arch-bluetooth-pulseaudio
pkgname=arch-bluetooth-pulseaudio
pkgver=1.0
pkgrel=1

pkgdesc='Arch Bluetooth Pulseaudio configuration'
arch=('any')
url='https://wiki.archlinux.org/index.php/bluetooth#Audio'
license=('custom')

source=(
    'etc-pulse-custom.pa'
)


package_arch-bluetooth-pulseaudio() {
    pkgdesc='Bluetooth Pulseaudio fixes per Arch wiki'
    depends=(
        'alsa-utils'
        'bluez-utils'
        'blueberry'
        'pulseaudio-alsa'
        'pulseaudio-bluetooth'
        'pavucontrol'
    )
    install=arch-bluetooth-pulseaudio.install

    install -Dm0644 etc-pulse-custom.pa "$pkgdir"/etc/pulse/custom.pa
}


md5sums=('a39be2c92ed14a937e33818cea8a5517')
