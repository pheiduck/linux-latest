# Maintainer: Jonathon Fernyhough <jonathon at_manjaro dot.org>

pkgbase=linux-latest
pkgver=5.1
pkgrel=1
pkgname=(
	"${pkgbase}"
	"${pkgbase}-headers"
	"${pkgbase}-acpi_call"
	"${pkgbase}-bbswitch"
	"${pkgbase}-broadcom-wl"
	"${pkgbase}-catalyst"
	"${pkgbase}-ndiswrapper"
	"${pkgbase}-nvidia"
	"${pkgbase}-nvidia-340xx"
	"${pkgbase}-nvidia-390xx"
	"${pkgbase}-nvidiabl"
	"${pkgbase}-r8168"
	"${pkgbase}-rt3562sta"
	"${pkgbase}-tp_smapi"
	"${pkgbase}-vhba-module"
	"${pkgbase}-virtualbox-guest-modules"
	"${pkgbase}-virtualbox-host-modules"
	"${pkgbase}-zfs"
)
# Set this as default for the extramodules, override for kernel and headers
groups=(linux-latest-extramodules)
arch=('any')
url="https://www.manjaro.org/"
license=('GPL')
_kernelver="${pkgver/\./}"

package_linux-latest() {
	pkgdesc="The latest kernel and modules (metapackage)"
	depends=("linux${_kernelver}")
	groups=()
}

package_linux-latest-headers() {
	pkgdesc="Header files and scripts for building modules for the latest kernel (metapackage)"
	depends=("linux${_kernelver}-headers")
	groups=()
}

package_linux-latest-acpi_call(){
	pkgdesc="A linux kernel module that enables calls to ACPI methods through /proc/acpi/call (metapackage)"
	depends=("linux${_kernelver}-acpi_call")
}

package_linux-latest-bbswitch(){
	pkgdesc="Kernel module allowing to switch dedicated graphics card on Optimus laptops (metapackage)"
	depends=("linux${_kernelver}-bbswitch")
}

package_linux-latest-broadcom-wl(){
	pkgdesc="Broadcom 802.11 Linux STA wireless driver BCM43142 (metapackage)"
	depends=("linux${_kernelver}-broadcom-wl")
}

package_linux-latest-catalyst(){
	pkgdesc="AMD/ATI Catalyst drivers for linux. fglrx kernel module only (metapackage)"
	depends=("linux${_kernelver}-catalyst")
}

package_linux-latest-ndiswrapper(){
	pkgdesc="Module for NDIS (Windows Network Drivers) drivers supplied by vendors (metapackage)"
	depends=("linux${_kernelver}-ndiswrapper")
}

package_linux-latest-nvidia(){
	pkgdesc="NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia")
}

package_linux-latest-nvidia-340xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-304xx")
}

package_linux-latest-nvidia-390xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-340xx")
}

package_linux-latest-nvidiabl(){
	pkgdesc="Driver to adjust display backlight on modern mobile NVidia graphics adapters (metapackage)"
	depends=("linux${_kernelver}-nvidiabl")
}

package_linux-latest-r8168(){
	pkgdesc="A kernel module for Realtek 8168 network cards (metapackage)"
	depends=("linux${_kernelver}-r8168")
}

package_linux-latest-rt3562sta(){
	pkgdesc="Ralink RT3562 PCI WLAN adaptors kernel module (metapackage)"
	depends=("linux${_kernelver}-rt3562sta")
}

package_linux-latest-tp_smapi(){
	pkgdesc="Modules for ThinkPad's SMAPI functionality (metapackage)"
	depends=("linux${_kernelver}-tp_smapi")
}

package_linux-latest-vhba-module(){
	pkgdesc="Kernel module that emulates SCSI devices (metapackage)"
	depends=("linux${_kernelver}-vhba-module")
}

package_linux-latest-virtualbox-guest-modules(){
	pkgdesc="Guest kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-guest-modules")
}

package_linux-latest-virtualbox-host-modules(){
	pkgdesc="Host kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-host-modules")
}

package_linux-latest-zfs(){
	pkgdesc="Kernel modules for the Zettabyte File System (metapackage)"
	depends=("linux${_kernelver}-zfs")
}
