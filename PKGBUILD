# Maintainer: McQueen <clear3239@yahoo.com>
_pkgname=arch-logo-dark
pkgname=arch-logo-dark-wallpapers
pkgver=1.0.1
pkgrel=1
pkgdesc='Collection of Arch Logo Dark Wallpapers'
arch=(any)
url='https://ffwallpaper.com/arch-linux.html'
_url="https://github.com/MMcQueenGNU"
license=('CC-BY-SA')
source=("$_url/$pkgname/archive/refs/tags/v$pkgver.tar.gz")

md5sums=('')

package() {

	cd "$srcdir/$pkgname-$pkgver/$_pkgname"

	# Creating needed directories
	install -dm755 "${pkgdir}/usr/share/backgrounds/$_pkgname/"

	# Wallpapers
	local wallpaper
	for wallpaper in *; do
		install -m755 "$srcdir/$pkgname-$pkgver/$_pkgname/${wallpaper}" "$pkgdir/usr/share/backgrounds/$_pkgname/${wallpaper}"
	done
}
