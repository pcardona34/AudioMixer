include $(GNUSTEP_MAKEFILES)/common.make

PACKAGE_NAME = AudioMixer
VERSION = 0.7.3
APP_NAME = AudioMixer
AudioMixer_MAIN_MODEL_FILE = AudioMixer.gorm
AudioMixer_APPLICATION_ICON = Mixer.tiff

AudioMixer_OBJC_FILES = \
main.m \
AppController.m

AudioMixer_RESOURCE_FILES = \
Mixer.tiff

# Localization
AudioMixer_LANGUAGES= English French
AudioMixer_LOCALIZED_RESOURCE_FILES = \
InfoPlist.strings \
Localizable.strings \
AudioMixer.gorm

# GNUSTEP_TARGET_OS is defined to `linux-gnueabi' on armel and
# `linux-gnuspep' on powerpcspe.
ifneq (,$(findstring linux-gnu,$(GNUSTEP_TARGET_OS)))
ADDITIONAL_GUI_LIBS = -lasound
endif

include $(GNUSTEP_MAKEFILES)/application.make
