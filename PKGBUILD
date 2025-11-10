pkgname=varia-keyring
pkgver=20251110
pkgrel=2
pkgdesc="Pacman keyring for Varia Linux"
arch=('any')
url="https://varia-linux.github.io/repo"
license=('GPL')
depends=('pacman>=7.0.0')
install=varia-keyring.install

source=(
    'varia-repo.gpg'
    'public_key_fingerprints'
)
sha256sums=('5486d307405776184bb588fef95d4ad37ffe1b2e39b99afe01f6b732e23f7079'
            'b29a32fa4f578271f178ce505702a03b12a42a55c4e7f59ae5086ed86d979ac1')

package() {
    install -Dm644 varia-repo.gpg "$pkgdir/usr/share/keyrings/$pkgname/myrepo.gpg"
    install -Dm644 public_key_fingerprints "$pkgdir/usr/share/keyrings/$pkgname/public_key_fingerprints"
}