## TWRP device tree for Samsung Galaxy S4 Mini Sprint
## serranoltespr

Add to `.repo/local_manifests/serranoltespr.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="LineageOS/android_device_qcom_common" path="device/qcom/common" remote="github" revision="cm-14.1" />
  <project name="LineageOS/android_kernel_samsung_msm8930-common" path="kernel/samsung/msm8930-common" remote="github" revision="cm-14.1" />
  <project name="TeamWin/android_device_samsung_serranoltespr" path="device/samsung/serranoltespr" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_serranoltespr-eng
mka recoveryimage
```

