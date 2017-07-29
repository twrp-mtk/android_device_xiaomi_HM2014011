## TWRP device tree for Xiaomi Redmi 1S TD (HM2014011)

Add to `.repo/local_manifests/HM2014011.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/xiaomi/HM2014011" name="android_device_xiaomi_HM2014011" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_HM2014011-eng
make -j5 recoveryimage
```
Kernel source is available at: https://github.com/ferhung-mtk/android_kernel_Xiaomi_HM2014011
