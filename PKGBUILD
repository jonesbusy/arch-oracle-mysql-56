# Maintainer: Valentin Delaye <jonesbusy@gmail.com>
# Contributor: Valentin Delaye <jonesbusy@gmail.com>
pkgname=oracle-mysql
pkgver=5.6.21
pkgrel=0
pkgdesc="Oracle MySQL 5.6"
url="http://www.mysql.com/"
arch=('x86_64')
license=('GPLv2')
depends=('mariadb')
optdepends=()
makedepends=()
conflicts=()
groups=('mysql')
replaces=()
options=(!strip !zipman !purge)
backup=()
install='mysql56.install'
source=("${pkgname}.tar.gz::http://cdn.mysql.com/Downloads/MySQL-5.6/mysql-5.6.21-linux-glibc2.5-$CARCH.tar.gz")
md5sums=('79f9a54bdc3731fd4bdf22db77f27ca7')

build() {
    cd "${srcdir}"
    mv "mysql-5.6.21-linux-glibc2.5-$CARCH" "opt/${pkgname}"
}

package() {
  cp -R "${srcdir}/usr" "${pkgdir}/usr"
  cp -R "${srcdir}/opt" "${pkgdir}/opt" 
}