# Contributor: jorge_barroso <jorge.barroso.11@gmail.com>"
# Contributor: mar77i <mysatyre at gmail dot com>"

_debname=iceweasel
_debver=16.0.1
_debrel=1
_debrepo=http://ftp.debian.org/debian/pool/main/

pkgname=iceweasel-i18n-nso
pkgver=$_debver
pkgrel=1
groups=('iceweasel-i18n')
pkgdesc="Language packs for Debian Iceweasel."
arch=('any')
url="http://www.geticeweasel.org/"
license=('MPL')
depends=("iceweasel>=$_debver")

source=("$_debrepo/${_debname:0:1}/$_debname/$_debname-l10n-nso_${_debver}-${_debrel}_all.deb")
md5sums=(d5e5b6d7f4018b34fe01980548221332)

build() {
	cd "$srcdir"
	bsdtar xf "${source##*/}"
	cd "$pkgdir"
	tar Jxf "$srcdir"/data.tar.xz
}


