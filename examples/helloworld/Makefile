include $(TOPDIR)/rules.mk

PKG_NAME:=helloworld
PKG_VERSION:=1.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/helloworld
	SECTION:=examples
	CATEGORY:=Examples
	TITLE:=Hello, World!
endef

define Package/helloworld/description
	A simple "Hello, world!" -application.
endef

define Package/helloworld/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/helloworld $(1)/usr/bin
endef

$(eval $(call BuildPackage,helloworld))