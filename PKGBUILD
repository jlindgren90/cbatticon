# Maintainer: John Lindgren <john@jlindgren.net>

pkgname=cbatticon-qt
pkgver=1.6.10
pkgrel=1
pkgdesc='Lightweight battery icon for the system tray (Qt 6 version)'
arch=(x86_64)
url='https://github.com/jlindgren90/cbatticon'
license=(GPL2)
depends=(qt6-base libnotify)
conflicts=(cbatticon)

build() {
    cd ..
    make WITH_NOTIFY=1 WITH_QT6=1
}

package() {
    cd ..
    make DESTDIR="${pkgdir}" PREFIX=/usr install
}
