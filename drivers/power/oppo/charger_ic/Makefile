ifeq ($(CONFIG_OPPO_CHARGER_MTK),y)
ifeq ($(CONFIG_OPPO_CHARGER_6750T),y)
else ifeq ($(CONFIG_OPPO_CHARGER_MTK6763),y)
else ifeq ($(CONFIG_OPPO_CHARGER_MTK6771),y)
else
	include $(srctree)/drivers/misc/mediatek/Makefile.custom
endif
	ifeq ($(CONFIG_MTK_HAFG_20),y)
		obj-y	+= oppo_battery_mtk_fg_20.o
else ifeq ($(CONFIG_OPPO_CHARGER_MTK6763),y)
obj-y	+= oppo_battery_mtk6763.o
else ifeq ($(CONFIG_OPPO_CHARGER_MTK6771),y)
obj-y	+= oppo_bq24190.o
obj-y	+= oppo_bq25890h.o
obj-y	+= oppo_battery_mtk6771.o
obj-y   += smb1351-charger.o
	else
		obj-y	+= oppo_battery_mtk.o
	endif
	obj-y	+= oppo_bq2202a.o
	obj-y	+= oppo_bq24196.o
else ifeq ($(CONFIG_OPPO_MSM8953N_CHARGER),y)
	obj-y	+= oppo_battery_msm8953_N.o
else ifeq ($(CONFIG_OPPO_MSM8953_CHARGER),y)
	obj-y	+= oppo_battery_msm8953.o
else ifeq ($(CONFIG_OPPO_MSM8998_CHARGER),y)
	obj-y	+= oppo_battery_msm8998.o
else ifeq ($(CONFIG_OPPO_MSM8998O_CHARGER),y)
	obj-y	+= oppo_battery_msm8998_O.o
else ifeq ($(CONFIG_OPPO_CHARGE_450_O),y)
	obj-y	+= oppo_battery_sdm450_O.o
else
	obj-y	+= oppo_battery_msm8976.o
endif 

