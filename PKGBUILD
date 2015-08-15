# Maintainer: Limao Luo <luolimao+AUR@gmail.com>

pkgname=dropbox-dark-panel-icons
pkgver=1.0
pkgrel=10
pkgdesc="Notification icons for Dropbox for themes with dark panels."
arch=(any)
url=https://forums.dropbox.com/topic.php?id=7818
license=(CCPL:by-3.0)
depends=(dropbox hicolor-icon-theme)
conflicts=(dropbox-{light-panel,humanity{,-dark}}-icons)
install=icons.install
source=($pkgname.tar.gz::'https://dl.dropbox.com/u/62148/Misc/Dropbox Dark Panel.tar.gz?dl=1')
sha256sums=('058d57d6db040b3394bc309c37490f7e2d874fc1955d5c4cb7210223984d3680')
sha512sums=('6416022bf3cf8bdd40489566260fdd07f13959f54cc6c96a4169f42669058efb7eaa595ef5c1f68ddfa8b3aced059adbeb176265373b5a470fb0eae6b42be5d8')

package() {
    cd "$srcdir"/icons/
    for i in *.png; do
        install -Dm644 $i "$pkgdir"/usr/share/icons/hicolor/16x16/status/dropboxstatus-$i
    done
}
