## TWRP device tree for Samsung Galaxy S4 (Value Edition)
## jfvelte

Add to `.repo/local_manifests/jfvelte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="TeamWin/android_device_samsung_jfvelte" path="device/samsung/jfvelte" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_jfvelte-eng
mka recoveryimage
```

Kernel source: https://github.com/jfvelte-dev/android_kernel_samsung_jf/tree/cm-14.1
