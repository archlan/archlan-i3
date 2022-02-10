# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    PKGBUILD                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: Lanhild <archlan@protonmail.com>           +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/01/23 12:22:12 by Lanhild           #+#    #+#              #
#    Updated: 2022/02/10 17:12:04 by Lanhild          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

# Maintainer: Lanhild <lanhild@pm.me>

pkgname=archlan-i3
pkgver=1.1
pkgrel=6
pkgdesc="i3wm Configurations for ArchLan"
url="https://github.com/archlan/archlan-i3"
arch=('any')
license=('GPL3')
makedepends=('git')
depends=('i3-gaps' 'hsetroot' 'pywal' 'rofi' 'alacritty' 'dunst' 'picom-ibhagwan-git' 'polybar')
conflicts=()
groups=('archlan-de')
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
	cp -rf ${srcdir}/alacritty 		"$_config"
	cp -rf ${srcdir}/dunst 			"$_config"
	cp -rf ${srcdir}/polybar 		"$_config"
	cp -rf ${srcdir}/rofi 			"$_config"
	cp -rf ${srcdir}/scripts 		"$_config"
	cp -rf ${srcdir}/wallpapers 	"$_config"

	chmod -R 755 "$_config"/scripts

	install -Dm 644 config   		"$_config"/config
	install -Dm 644 picom.conf   	"$_config"/picom.conf
}