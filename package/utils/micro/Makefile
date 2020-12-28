#
# Copyright (C) 2007-2016 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=micro
PKG_VERSION:=2.0.8
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.xz
PKG_SOURCE_URL:=https://github.com/zyedidia/micro/archive/v$(PKG_VERSION).tar.gz
PKG_HASH:=3e1b7483aa2afffa8afc2c710e22541961ac3de5e026efb4bdddc8ade00d4de0

PKG_LICENSE:=GPL-3.0-or-later
PKG_LICENSE_FILES:=COPYING
PKG_MAINTAINER:=Thaison Nguyen <thieson08@me.com>
# PKG_CPE_ID:=cpe:/a:gnu:nano

PKG_INSTALL:=1
PKG_BUILD_PARALLEL:=1

include $(INCLUDE_DIR)/package.mk

define Package/nano
  SUBMENU:=Editors
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=micro aims to be somewhat of a successor to the nano editor
  URL:=https://micro-editor.github.io/
  DEPENDS:=
endef

define Package/micro/description
  micro is a terminal-based text editor that aims to be easy to use and intuitive,
  while also taking advantage of the capabilities of modern terminals.
endef

CONFIGURE_ARGS +=

CONFIGURE_VARS +=

define Package/micro/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(CP) $(PKG_INSTALL_DIR)/usr/bin/$(PKG_NAME) $(1)/usr/bin/
endef

$(eval $(call BuildPackage,micro))
