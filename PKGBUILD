# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Anatol Pomozov <anatol.pomozov@gmail.com>
# Contributor: Alfredo Palhares <masterkorp@masterkorp.net>
# Contributor: Alexsandr Pavlov <kidoz@mail.ru>

_gemname=mime-types
pkgname=ruby-$_gemname-1.16
pkgver=1.16
pkgrel=4
pkgdesc='Manages a MIME Content-Type database that will return the Content-Type for a given filename.'
arch=(any)
url='http://mime-types.rubyforge.org/'
license=('GPL2' MIT 'PerlArtistic')
depends=(ruby)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('dc9c8d0eca668c18c21302b439645c20327da3ab')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
