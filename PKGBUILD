# Maintainer: pdq <pdq@localhost>
pkgname=brutaldoom
pkgver=19
pkgrel=1
pkgdesc="Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines."
arch=(any)
url="http://www.moddb.com/mods/brutal-doom"
license=('GPL3')
depends=('zandronum')
optdepends=('doomseeker')
makedepends=('git')
source=('brutal19.zip::http://www.moddb.com/downloads/mirror/61237/102/ca7db3921bdacaf2a2227d7264cfd240'
        'DoomMetalVol4.zip::http://www.moddb.com/downloads/mirror/61238/102/0d3f85cb2e4bc674f5b7d697c27309cb'
        'git://github.com/idk/brutaldoom.git')
sha512sums=('5b87f3a849fc61561fc971c24c1cc2840fc42e063ef2a946cfd11dc77a3d0cbd310750836f2b1b8be86e1c3211a1b426447ef2917caef3adc8cbef50f6f321b2'
            'b1180910025e8b8f065c56518fb1556678ef5c6062dc527e1f3e54dfa039e82f8e49bb1997ccf06a07e451576fbe35c321773eb7dbb7f62b1654b59cb9e07f32'
            'SKIP')

install=$pkgname.install

package() {
	install -d "$pkgdir/usr/share/games/$pkgname"
	msg2 "Installing brutal19.pk3 and DoomMetalVol4.wad..."
	N="brutal19.pk3";           install -Dm644 "$srcdir/$N" "$pkgdir/usr/share/games/$pkgname/$N"
	N="DoomMetalVol4.wad";      install -Dm644 "$srcdir/$N" "$pkgdir/usr/share/games/$pkgname/$N"
	N="brutal19.txt";           install -Dm644 "$srcdir/$N" "$pkgdir/usr/share/games/$pkgname/$N"
	N="brutaldoom credits.txt"; install -Dm644 "$srcdir/$N" "$pkgdir/usr/share/games/$pkgname/$N"

	msg2 "Installing configuration files..."
	N="zandronum.ini";          install -Dm644 "$srcdir/$pkgname/$N" "$pkgdir/usr/share/games/$pkgname/$N"
}
