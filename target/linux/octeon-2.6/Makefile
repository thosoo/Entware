#
# Copyright (C) 2011-2017 Entware
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

ARCH:=mips64
BOARD:=octeon-2.6
BOARDNAME:=Entware (octeon, soft float, kernel-2.6.36)
FEATURES:=gpio usb audio pci
KERNEL_PATCHVER:=2.6.36
CPU_TYPE:=octeonplus
DEFAULT_PACKAGES := toolchain

include $(INCLUDE_DIR)/target.mk

define Target/Description
	Build Software Repository for OcteonPlus.
endef

$(eval $(call BuildTarget))
