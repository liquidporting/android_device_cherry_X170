## TWRP device tree for Cherry Mobile Me Vibe (X170)

Add to `.repo/local_manifests/X170.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/cherry/X170" name="android_device_cherry_X170" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_X170-eng
make -j5 recoveryimage
```
