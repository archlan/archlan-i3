# Maintainer: Lanhild <lanhild@pm.me>

pkgname=archlan-i3
pkgver=1.0
pkgrel=1
pkgdesc="i3wm Configurations for ArchLan"
url="https://github.com/archlan/archlan-i3"
arch=('any')
license=('GPL3')
makedepends=('git')
depends=('archlan-skel' 'i3-gaps' 'hsetroot')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
install="${pkgname}.install"

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	local _config=${pkgdir}/etc/skel/.config/i3
	mkdir -p "$_config"

	# Copy i3wm config files
	cp -r ${srcdir}/alacritty 		"$_config"
	cp -r ${srcdir}/bin 			"$_config"
	cp -r ${srcdir}/polybar 		"$_config"
	cp -r ${srcdir}/rofi 			"$_config"
	cp -r ${srcdir}/wallpapers 		"$_config"

	chmod +x "$_config"/bin/*
	chmod +x "$_config"/rofi/bin/*

	install -Dm 644 config   		"$_config"/config
	install -Dm 644 picom.conf   	"$_config"/picom.conf
}