# Reference: <https://postmarketos.org/devicepkg>
pkgname="device-motorola-ginna"
pkgdesc="Motorola Moto e 2020, codename 'ginna"
pkgver=1
pkgrel=0
url="https://github.com/orowith2os/motorola-ginna-docs"
license="MIT"
arch="aarch64"
options="!check !archcheck"
depends="postmarketos-base mkbootimg linux-postmarketos-qcom-msm8953 soc-qcom-msm8953"
makedepends="devicepkg-dev"
source="deviceinfo"

build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
}
