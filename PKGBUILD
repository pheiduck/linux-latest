# Maintainer: Philip Heiduck <pheiduck[at]forum[dot]manjaro[dot]org>
# Maintainer: Philip Müller <philm[at]manjaro[dot]org>
# Maintainer: Bernhard Landauer <bernhard[at]manjaro[dot]org>
# Maintainer: Helmut Stult <helmut[at]manjaro[dot]org>

pkgbase=linux-latest
pkgver=6.7
pkgrel=3
pkgname=(
	"${pkgbase}"
	"${pkgbase}-headers"
	"${pkgbase}-acpi_call"
	"${pkgbase}-bbswitch"
	"${pkgbase}-broadcom-wl"
	"${pkgbase}-nvidia"
 	"${pkgbase}-nvidia-470xx"
	"${pkgbase}-nvidia-390xx"
	"${pkgbase}-r8168"
	"${pkgbase}-rtl8723bu"
	"${pkgbase}-tp_smapi"
	"${pkgbase}-vhba-module"
	"${pkgbase}-virtualbox-host-modules"
	"${pkgbase}-zfs"
)
# Set this as default for the extramodules, override for kernel and headers
groups=(linux-latest-extramodules)
arch=('any')
url="https://www.manjaro.org/"
license=('GPL')
_kernelver="${pkgver/\./}"

# EOL kernels between last LTS and latest
eol=()

package_linux-latest() {
	pkgdesc="The latest kernel and modules (metapackage)"
	depends=("linux${_kernelver}")
	groups=()
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}")
		conflicts+=("linux${kernel}")
	done
}

package_linux-latest-headers() {
	pkgdesc="Header files and scripts for building modules for the latest kernel (metapackage)"
	depends=("linux${_kernelver}-headers")
	groups=()
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-headers")
		conflicts+=("linux${kernel}-headers")
	done
}

package_linux-latest-acpi_call(){
	pkgdesc="A linux kernel module that enables calls to ACPI methods through /proc/acpi/call (metapackage)"
	depends=("linux${_kernelver}-acpi_call")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-acpi_call")
		conflicts+=("linux${kernel}-acpi_call")
	done
}

package_linux-latest-bbswitch(){
	pkgdesc="Kernel module allowing to switch dedicated graphics card on Optimus laptops (metapackage)"
	depends=("linux${_kernelver}-bbswitch")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-bbswitch")
		conflicts+=("linux${kernel}-bbswitch")
	done
}

package_linux-latest-broadcom-wl(){
	pkgdesc="Broadcom 802.11 Linux STA wireless driver BCM43142 (metapackage)"
	depends=("linux${_kernelver}-broadcom-wl")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-broadcom-wl")
		conflicts+=("linux${kernel}-broadcom-wl")
	done
}

package_linux-latest-nvidia-390xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-390xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-390xx")
		conflicts+=("linux${kernel}-nvidia-390xx")
	done
}

package_linux-latest-nvidia-470xx(){
        pkgdesc="NVIDIA drivers for Linux (metapackage)"
        depends=("linux${_kernelver}-nvidia-470xx")
        for kernel in "${eol[@]}"; do
                replaces+=("linux${kernel}-nvidia-470xx")
                conflicts+=("linux${kernel}-nvidia-470xx")
        done
}

package_linux-latest-nvidia(){
        pkgdesc="NVIDIA drivers for Linux (metapackage)"
        depends=("linux${_kernelver}-nvidia")
        for kernel in "${eol[@]}"; do
                replaces+=("linux${kernel}-nvidia")
                conflicts+=("linux${kernel}-nvidia")
        done
}

package_linux-latest-r8168(){
	pkgdesc="A kernel module for Realtek 8168 network cards (metapackage)"
	depends=("linux${_kernelver}-r8168")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-r8168")
		conflicts+=("linux${kernel}-r8168")
	done
}

package_linux-latest-rtl8723bu(){
	pkgdesc="Realtek 8723bu network card kernel module (metapackage)"
	depends=("linux${_kernelver}-rtl8723bu")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-rtl8723bu")
		conflicts+=("linux${kernel}-rtl8723bu")
	done
}

package_linux-latest-tp_smapi(){
	pkgdesc="Modules for ThinkPad's SMAPI functionality (metapackage)"
	depends=("linux${_kernelver}-tp_smapi")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-tp_smapi")
		conflicts+=("linux${kernel}-tp_smapi")
	done
}

package_linux-latest-vhba-module(){
	pkgdesc="Kernel module that emulates SCSI devices (metapackage)"
	depends=("linux${_kernelver}-vhba-module")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-vhba-module")
		conflicts+=("linux${kernel}-vhba-module")
	done
}

package_linux-latest-virtualbox-host-modules(){
	pkgdesc="Host kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-host-modules")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-virtualbox-host-modules")
		conflicts+=("linux${kernel}-virtualbox-host-modules")
	done
}

package_linux-latest-zfs(){
	pkgdesc="Kernel modules for the Zettabyte File System (metapackage)"
	depends=("linux${_kernelver}-zfs")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-zfs")
		conflicts+=("linux${kernel}-zfs")
	done
}
