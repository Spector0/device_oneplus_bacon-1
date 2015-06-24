Device tree for One+One

Copyright 2015, The CyanogenMod Project

## Device Handler
This is Slim Roms Device Handler

Add the following to enable it for your device

To device.mk

PRODUCT_PACKAGES += \ DeviceHandler

and To overlay/frameworks/base/core/res/res/values/config.xml add:

<!-- The list absolute paths of jar/apk files containing the device specific handlers,
     delimited by File.pathSeparator, which defaults to ":" on Android -->
<string name="config_deviceKeyHandlerLib" translatable="false">/system/app/DeviceHandler.apk</string>

<!-- Full qualified name of the class that implements
     com.android.internal.os.DeviceKeyHandler interface. -->
<string name="config_deviceKeyHandlerClass" translatable="false">com.broken.device.KeyHandler</string>
