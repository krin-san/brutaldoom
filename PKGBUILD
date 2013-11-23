# Maintainer: pdq <pdq@localhost>
pkgname=brutaldoom
pkgver=18
pkgrel=1
pkgdesc="Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines."
arch=(any)
url="http://www.moddb.com/downloads/brutal-doom-version-181"
license=('GPL3')
depends=('doomseeker' 'zandronum')
optdepends=()
makedepends=('git')

source=("http://www.theultimatedoom.com/download/brutalv0${pkgver}a.zip" "http://mooos.org/mooOS-utils/doommetalvol4.tar.gz")
md5sums=('fc0d6f2a63aeb3f9028221bd9ab77ec5'
		 '67975e13059aceb7fa5d93d3d91de99b')

_gitroot="git://github.com/idk/brutaldoom.git"
_gitname="brutaldoom"

install=$pkgname.install

build() {
	cd "$srcdir"
	msg "Connecting to GIT server...."
	if [ -d $_gitname-build ] ; then
		cd $_gitname-build && git pull origin
		msg "The local files are updated."
	else
		msg "Starting make..."
		git clone "$_gitroot" "$srcdir/$_gitname-build"
	fi
}

package() {
	cd ${srcdir}
	mkdir -p "$pkgdir/usr/share/games/$pkgname"

	msg2 "Installing brutalv0${pkgver}a.pk3 and doommetalvol4.wad..."
	install -Dm644 "$srcdir/brutalv0${pkgver}a.pk3" "$pkgdir/usr/share/games/$pkgname/brutalv0${pkgver}a.pk3"
	install -Dm644 "$srcdir/doommetalvol4.wad" "$pkgdir/usr/share/games/$pkgname/doommetalvol4.wad"

	msg2 "Installing configuration files..."
	cd "$srcdir/$_gitname-build"
	install -Dm644 "$srcdir/$_gitname-build/zandronum.ini" "$pkgdir/usr/share/games/$pkgname/zandronum.ini"
	install -Dm644 "$srcdir/$_gitname-build/brutalv018a changelog.txt" "$pkgdir/usr/share/games/$pkgname/brutalv018a_changelog.txt"

	rm -rf "$srcdir/$_gitname-build"
}
