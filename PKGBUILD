# Maintainer: pdq <pdq@localhost>
pkgname=brutaldoom
pkgver=18
pkgrel=2
pkgdesc="Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines."
arch=(any)
url="http://www.moddb.com/downloads/brutal-doom-version-18a"
license=('GPL3')
depends=('zandronum')
optdepends=('doomseeker')
makedepends=('git')
source=('http://www.moddb.com/downloads/mirror/51150/112/68fbdcea87118fa9438d40a40c74d7a8'
        'http://www.moddb.com/downloads/mirror/61238/112/cd99ffe9d2f7903526d70ad1be065325'
        'git://github.com/idk/brutaldoom.git')
sha512sums=('c940afc94317937b9b91da071440053d426b82a43d9f756aa2b3c899d7e966da06cc2d4226258f5b074ea2da780043a5cecfa2e0ba9e21d4c0aee14d282e8d60'
            'b1180910025e8b8f065c56518fb1556678ef5c6062dc527e1f3e54dfa039e82f8e49bb1997ccf06a07e451576fbe35c321773eb7dbb7f62b1654b59cb9e07f32'
            'SKIP')

install=$pkgname.install

package() {
	install -d "$pkgdir/usr/share/games/$pkgname"
	msg2 "Installing brutalv018a.pk3 and DoomMetalVol4.wad..."
	install -Dm644 "$srcdir/brutalv018a.pk3" "$pkgdir/usr/share/games/$pkgname/brutalv018a.pk3"
	install -Dm644 "$srcdir/DoomMetalVol4.wad" "$pkgdir/usr/share/games/$pkgname/DoomMetalVol4.wad"
	install -Dm644 "$srcdir/brutalv018a changelog.txt" "$pkgdir/usr/share/games/$pkgname/brutalv018a_changelog.txt"
	install -Dm644 "$srcdir/Credits.txt" "$pkgdir/usr/share/games/$pkgname/Credits.txt"

	msg2 "Installing configuration files..."
	install -Dm644 "$srcdir/$pkgname/zandronum.ini" "$pkgdir/usr/share/games/$pkgname/zandronum.ini"
}
