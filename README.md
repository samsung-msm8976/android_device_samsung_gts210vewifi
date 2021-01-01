## TWRP device tree for Samsung Galaxy Tab S2 9.7 Wi-Fi (gts210vewifi)
## gts210vewifi

Add to `.repo/local_manifests/gts210vewifi.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ripee/android_device_samsung_gts210vewifi" path="device/samsung/gts210vewifi" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_gts210vewifi-eng
mka recoveryimage
```

Kernel source: https://github.com/LineageOS/android_kernel_samsung_msm8976/tree/4664546f2b58d616ae66c109dea862cf928fb5d4
