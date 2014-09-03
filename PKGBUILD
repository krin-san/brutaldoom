# Maintainer: pdq <pdq@localhost>
pkgname=brutaldoom
pkgver=19
pkgrel=2
pkgdesc="Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines."
arch=(any)
url="http://www.moddb.com/downloads/brutal-doom-version-19"
license=('GPL3')
depends=('doomseeker' 'zandronum')
optdepends=()
makedepends=('git')
source=("http://www.moddb.com/downloads/mirror/61237/112/727339ae0978747dc6d3a5109ca9ea5e" "http://www.moddb.com/downloads/mirror/61238/112/cd99ffe9d2f7903526d70ad1be065325")
sha512sums=('5b87f3a849fc61561fc971c24c1cc2840fc42e063ef2a946cfd11dc77a3d0cbd310750836f2b1b8be86e1c3211a1b426447ef2917caef3adc8cbef50f6f321b2'
		 'b1180910025e8b8f065c56518fb1556678ef5c6062dc527e1f3e54dfa039e82f8e49bb1997ccf06a07e451576fbe35c321773eb7dbb7f62b1654b59cb9e07f32')

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

	msg2 "Installing brutal${pkgver}.pk3 and DoomMetalVol4.wad..."
	install -Dm644 "$srcdir/brutal${pkgver}.pk3" "$pkgdir/usr/share/games/$pkgname/brutal${pkgver}.pk3"
	install -Dm644 "$srcdir/DoomMetalVol4.wad" "$pkgdir/usr/share/games/$pkgname/DoomMetalVol4.wad"
	install -Dm644 "$srcdir/$_gitname-build/brutal19.txt" "$pkgdir/usr/share/games/$pkgname/brutal19.txt"
	install -Dm644 "$srcdir/$_gitname-build/brutaldoom credits.txt" "$pkgdir/usr/share/games/$pkgname/brutaldoom_credits.txt"
	install -Dm644 "$srcdir/$_gitname-build/Credits.txt" "$pkgdir/usr/share/games/$pkgname/Credits.txt"

	msg2 "Installing configuration files..."
	cd "$srcdir/$_gitname-build"
	install -Dm644 "$srcdir/$_gitname-build/zandronum.ini" "$pkgdir/usr/share/games/$pkgname/zandronum.ini"

	rm -rf "$srcdir/$_gitname-build"
}
