# Contributor: maz-1 <loveayawaka(at)gmail(dot)com>

pkgname=gimp-photoshop-brush
pkgver=1.0
pkgrel=1
pkgdesc="A Gimp plugin for loading photoshop brushes"
url="http://registry.gimp.org/node/126"
arch=('i686' 'x86_64')
license=("GPL")
depends=('gimp')
makedepends=('pkgconfig')
source=(http://registry.gimp.org/files/abr.c)
md5sums=('1f9009dc8254615e9eafb67e3efb4842')

build() {
  cd $startdir/src
  gimptool-2.0 --build abr.c
  #install -D -m 755 ./abr $startdir/pkg/usr/lib/gimp/2.0/plug-ins/abr || return 1
}
package(){
  install -D -m 755 ./abr $startdir/pkg/usr/lib/gimp/2.0/plug-ins/abr || return 1
}

