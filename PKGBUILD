pkgname=git-htmldocs
pkgver=2.3.3
pkgrel=1
pkgdesc="Git HTML and plain text documentation pages"
arch=(any)
url="http://git-scm.com"
license=(GPL)  # For some Java script; don't know about most of it though
makedepends=(tar)
_file="$pkgname-$pkgver.tar.xz"
source=("https://www.kernel.org/pub/software/scm/git/$_file")
noextract=("$_file")
md5sums=(51d8388d9672acd518089c383ac06fa6)

package() {
    local DIR="$pkgdir/usr/share/doc/git-doc"
    install -d "$DIR"
    tar xf "$srcdir/$_file" -C "$DIR" --no-same-owner
    chmod -R +u "$DIR"
}
