export ARCHS = arm64
export GO_EASY_ON_ME = 1
INSTALL_TARGET_PROCESSES = SpringBoard

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = Meteorite
Meteorite_FILES = $(wildcard source/*.x source/*.m)
Meteorite_FRAMEWORKS = CoreLocation UIKit
Meteorite_PRIVATE_FRAMEWORKS = AppSupport
Meteorite_LIBRARIES = mryipc
Meteorite_CFLAGS = -fobjc-arc -Wno-error=typedef-redefinition
Meteorite_LDFLAGS = -undefined dynamic_lookup

include $(THEOS_MAKE_PATH)/tweak.mk

SUBPROJECTS += meteorite
include $(THEOS_MAKE_PATH)/aggregate.mk
