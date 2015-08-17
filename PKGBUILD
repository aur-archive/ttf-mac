# Maintainer: Guten Ye

pkgname=ttf-mac
pkgver=10.8.1
pkgrel=5
pkgdesc='Mac OS X TrueType fonts. Please consult https://github.com/GutenYe/aur/tree/master/ttf-mac for Installation.'
arch=('any')
url='http://www.apple.com/osx/'
license=('custom')
depends=('fontconfig')
makedepends=('fondu')
conflicts=('ttf-mac-fonts')
install='install'

###################################################################
#        Normal        Bold           Italic         Bold+Italic  #
###################################################################
source=(
	'Apple Braille.ttf'
	'Apple Braille Outline 6 Dot.ttf'
	'Apple Braille Outline 8 Dot.ttf'
	'Apple Braille Pinpoint 6 Dot.ttf'
	'Apple Braille Pinpoint 8 Dot.ttf'
	'Courier.dfont'
	'Geeza Pro.ttf' 'Geeza Pro Bold.ttf'
	'Geneva.dfont'
	'Helvetica.dfont'
	'HelveticaNeue.dfont'
	'HelveticaNeueDeskUI.ttc'
	'Keyboard.ttf'
	'LucidaGrande.ttc'
	'MarkerFelt.ttc'
	'Menlo.ttc'
	'Monaco.dfont'
	'Symbol.ttf'
	'ThonburiBold.ttf'
	'Thonburi.ttf'
	'Times.dfont'
	'ZapfDingbats.ttf'
	)

build() {
  cd "$srcdir"

	fondu -force *.dfont
}

package() {
  cd "$srcdir"

  install -dm755 "$pkgdir/usr/share/fonts/TTF"
  install -m644 *.ttf *.ttc "$pkgdir/usr/share/fonts/TTF"
}

md5sums=('52455c11f8e401092df8f7c2e8912d8f'
         '23be6197029ed49537884d28c0ba4c10'
         '78ae851e6fe7dc652501fc62d3d9d6db'
         '0310cab5c0d8fe2a5bd54aacf0cfbd9a'
         '229b1af003990e9d577678f3a2f57c18'
         '56e90cce8c39cb79effe5a170a8b2572'
         '9bdf0da295eed72a4cd0e6bc72446bbf'
         '3af9b99a98e7edeff2d09bc94cb42003'
         'f8899861c19623bac0d4ca7506c48573'
         '885c66d7e4a39fb48d4edcb82b7ff96f'
         '9b0a306d4e9f880f75e8fbc6fb3abf97'
         'a9c3c9a855a2e53dc3212fc818c46e3b'
         'eca740e3da32bd12ac661a0af25f781e'
         'b27ea4f91a5a586d08d724bd66776af6'
         '116a49999fb3b9eac6ff0da90eb242e7'
         '21af790284394ed4d810b8e4d688985f'
         '9074c3d98f5f9a2795c4672892198166'
         'cd64343217ebef9d1959b0e70dee400b'
         '61f085541e3cc96bb42b0fed23f1a735'
         '62b0e8982d6bda8c45021e0cfe47658f'
         '7e7cfed05c8f4914baddde483b3a58c9'
         'd45b227261a2803cccff8e58fd284bc6')
