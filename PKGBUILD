# Maintainer: Jonathon Fernyhough <jonathon at_manjaro dot.org>

pkgbase=linux-latest
pkgver=5.2
pkgrel=2
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

# EOL kernels
eol=(
	317
	318
	319
	40
	41
	42
	43
	45
	46
	47
	48
	410
	411
	412
	413
	415
	416
	417
	418
	420
	50
)

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

package_linux-latest-catalyst(){
	pkgdesc="AMD/ATI Catalyst drivers for linux. fglrx kernel module only (metapackage)"
	depends=("linux${_kernelver}-catalyst")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-catalyst")
		conflicts+=("linux${kernel}-catalyst")
	done
}

package_linux-latest-ndiswrapper(){
	pkgdesc="Module for NDIS (Windows Network Drivers) drivers supplied by vendors (metapackage)"
	depends=("linux${_kernelver}-ndiswrapper")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-ndiswrapper")
		conflicts+=("linux${kernel}-ndiswrapper")
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

package_linux-latest-nvidia-340xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-304xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-304xx")
		conflicts+=("linux${kernel}-nvidia-304xx")
	done
}

package_linux-latest-nvidia-390xx(){
	pkgdesc="Legacy NVIDIA drivers for Linux (metapackage)"
	depends=("linux${_kernelver}-nvidia-340xx")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidia-340xx")
		conflicts+=("linux${kernel}-nvidia-340xx")
	done
}

package_linux-latest-nvidiabl(){
	pkgdesc="Driver to adjust display backlight on modern mobile NVidia graphics adapters (metapackage)"
	depends=("linux${_kernelver}-nvidiabl")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-nvidiabl")
		conflicts+=("linux${kernel}-nvidiabl")
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

package_linux-latest-rt3562sta(){
	pkgdesc="Ralink RT3562 PCI WLAN adaptors kernel module (metapackage)"
	depends=("linux${_kernelver}-rt3562sta")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-rt3562sta")
		conflicts+=("linux${kernel}-rt3562sta")
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

package_linux-latest-virtualbox-guest-modules(){
	pkgdesc="Guest kernel modules for VirtualBox (metapackage)"
	depends=("linux${_kernelver}-virtualbox-guest-modules")
	for kernel in "${eol[@]}"; do
		replaces+=("linux${kernel}-virtualbox-guest-modules")
		conflicts+=("linux${kernel}-virtualbox-guest-modules")
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

