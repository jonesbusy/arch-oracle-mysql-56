# Maintainer: Valentin Delaye <jonesbusy@gmail.com>
# Contributor: Valentin Delaye <jonesbusy@gmail.com>
pkgname=oracle-mysql
pkgver=5.6.21
pkgrel=1
pkgdesc="Oracle MySQL"
url="https://github.com/jonesbusy/arch-oracle-mysql-56"
arch=('i686' 'x86_64')
license=('GPL2')
depends=()
optdepends=()
makedepends=()
conflicts=()
groups=('mysql')
replaces=()
options=(!strip !zipman !purge)
backup=()
install='oracle-mysql.install'
source=("${pkgname}.tar.gz::http://cdn.mysql.com/Downloads/MySQL-5.6/mysql-5.6.21-linux-glibc2.5-$CARCH.tar.gz")
md5sums=('79f9a54bdc3731fd4bdf22db77f27ca7')

package() {
    rm -Rf "${srcdir}/${pkgname}"
    mv "${srcdir}/mysql-5.6.21-linux-glibc2.5-$CARCH" "${srcdir}/${pkgname}"
    mkdir "${pkgdir}/opt"
    cp -R "${pkgname}" "${pkgdir}/opt" 
    cp "${srcdir}/my.cnf.tmp" "${pkgdir}/opt/${pkgname}/my.cnf.tmp"
    cp -R "${srcdir}/usr" "${pkgdir}/usr"
}