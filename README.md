# local_manifests

For use with the main Lineage manifest.

```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="LineageOS/android_device_samsung_gts4lv" path="device/samsung/gts4lv" remote="github" />
  <project name="LineageOS/android_device_samsung_gts4lv-common" path="device/samsung/gts4lv-common" remote="github" />
  <project name="LineageOS/android_device_samsung_qcom-common" path="device/samsung/qcom-common" remote="github" />
  <project name="LineageOS/android_kernel_samsung_sdm670" path="kernel/samsung/sdm670" remote="github" revision="refs/heads/lineage-18.1" />
  <project name="LineageOS/android_hardware_samsung" path="hardware/samsung" remote="github" />

  <project name="TheMuppets/proprietary_vendor_samsung" path="vendor/samsung" remote="github" />

  <remove-project name="LineageOS/android_device_lineage_car" />
  <project path="device/lineage/car" name="tom-pratt/android_device_lineage_car" revision="main" />

  <remove-project name="LineageOS/android_device_samsung_gts4lv" />
  <project name="tom-pratt/android_device_samsung_gts4lv" path="device/samsung/gts4lv" remote="github" revision="main" />
</manifest>
```