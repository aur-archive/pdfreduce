# Maintainer: wombalton <wombalton@web.de>
# created by wombalton  <wombalton@web.de>

pkgname=pdfreduce
pkgver=1.0
pkgrel=3
pkgdesc="A bash script that tries to reduce the filesize of a PDF file by processing it through ghostscript."
arch=('any')
url="http://wombalton.ddns.net/pdfreduce.html"
license=('MIT')
depends=('ghostscript' 'pdftk')
makedepends=('')
changelog="changelog"
source=("http://wombalton.ddns.net/pdfreduce-1.0.tar.gz")
md5sums=('cd8f1c0fac7908237007069503b38f1a')

build() {
  cd "$srcdir"

    tar xvf pdfreduce-1.0.tar.gz
}

package() {
  cd "$srcdir"

  install -D -m 755 pdfreduce-1.0 "${pkgdir}/usr/bin/pdfreduce"

  install -D -m 644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
