#
# Makefile for physical layer USB drivers
#
GCOV_PROFILE_tegra-otg.o := y
GCOV_PROFILE_tegra-xotg.o := y

ccflags-$(CONFIG_USB_DEBUG) := -DDEBUG
subdir-ccflags-y += -Werror

obj-$(CONFIG_USB_PHY)			+= phy.o
obj-$(CONFIG_USB_OTG_WAKELOCK)		+= otg-wakelock.o

# transceiver drivers, keep the list sorted

obj-$(CONFIG_AB8500_USB)		+= phy-ab8500-usb.o
phy-fsl-usb2-objs			:= phy-fsl-usb.o phy-fsm-usb.o
obj-$(CONFIG_FSL_USB2_OTG)		+= phy-fsl-usb2.o
obj-$(CONFIG_ISP1301_OMAP)		+= phy-isp1301-omap.o
obj-$(CONFIG_MV_U3D_PHY)		+= phy-mv-u3d-usb.o
obj-$(CONFIG_NOP_USB_XCEIV)		+= phy-nop.o
obj-$(CONFIG_OMAP_CONTROL_USB)		+= phy-omap-control.o
obj-$(CONFIG_OMAP_USB2)			+= phy-omap-usb2.o
obj-$(CONFIG_OMAP_USB3)			+= phy-omap-usb3.o
obj-$(CONFIG_SAMSUNG_USBPHY)		+= phy-samsung-usb.o
obj-$(CONFIG_SAMSUNG_USB2PHY)		+= phy-samsung-usb2.o
obj-$(CONFIG_SAMSUNG_USB3PHY)		+= phy-samsung-usb3.o
obj-$(CONFIG_TWL4030_USB)		+= phy-twl4030-usb.o
obj-$(CONFIG_TWL6030_USB)		+= phy-twl6030-usb.o
ifeq ($(CONFIG_USB_EHCI_TEGRA),y)
obj-$(CONFIG_USB_EHCI_TEGRA)	+= phy-tegra-usb.o
obj-$(CONFIG_ARCH_TEGRA_11x_SOC)        += tegra11x_usb_phy.o
obj-$(CONFIG_ARCH_TEGRA_14x_SOC)        += tegra11x_usb_phy.o
obj-$(CONFIG_ARCH_TEGRA_12x_SOC)        += tegra11x_usb_phy.o
obj-$(CONFIG_ARCH_TEGRA_21x_SOC)        += tegra11x_usb_phy.o
endif
obj-$(CONFIG_USB_GPIO_VBUS)		+= phy-gpio-vbus-usb.o
obj-$(CONFIG_USB_ISP1301)		+= phy-isp1301.o
obj-$(CONFIG_USB_MSM_OTG)		+= phy-msm-usb.o
obj-$(CONFIG_USB_MV_OTG)		+= phy-mv-usb.o
obj-$(CONFIG_USB_MXS_PHY)		+= phy-mxs-usb.o
obj-$(CONFIG_USB_RCAR_PHY)		+= phy-rcar-usb.o
CFLAGS_tegra-otg.o		= -Werror
CFLAGS_tegra-xotg.o		= -Werror
obj-$(CONFIG_USB_TEGRA_OTG)	+= tegra-otg.o
obj-$(CONFIG_USB_TEGRA_XOTG)	+= tegra-xotg.o
obj-$(CONFIG_USB_ULPI)			+= phy-ulpi.o
obj-$(CONFIG_USB_ULPI_VIEWPORT)		+= phy-ulpi-viewport.o
