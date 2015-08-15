# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Contributor: Will Foran <foranw-upmc-edu>
pkgname=caret
pkgver=5.65
pkgrel=2
pkgdesc="structural and functional analyses of the cerebral and cerebellar cortex"
arch=("i686")
url="http://brainvis.wustl.edu/wiki/index.php/Caret:About"
license=('unknown')
depends=(qt vtk qwt netcdf)

source=(http://Rabbit:Carrot@brainmap.wustl.edu/pub/caret/${pkgname}_distribution_Linux32.v${pkgver}.zip)
md5sums=('8d318f3afbf3d7697d2df76ca109c978')

install='caret.install'
changelog='ChangeLog'

noextract=()

package() {
  mkdir -p $pkgdir/usr/{bin/,share/doc,share/$pkgname}

  install -m755    $srcdir/caret/bin_linux32/*               $pkgdir/usr/bin/ 
  cp -r            $srcdir/caret/{caret5_help,data_files}    $pkgdir/usr/share/$pkgname/
}

# vim:set ts=2 sw=2 et:
