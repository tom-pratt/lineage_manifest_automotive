# Sync

repo init -u https://github.com/tom-pratt/lineage_manifest_automotive.git -b main  
repo sync -c --no-clone-bundle --no-tags  

# Build

. build/envsetup  
lunch lineage_car_gts4lv-eng  
m bacon

# local_manifests

For use with the main Lineage manifest when generating snapshots.

```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="LineageOS/android_device_samsung_gts4lvwifi" path="device/samsung/gts4lvwifi" remote="github" />
  <project name="LineageOS/android_device_samsung_gts4lv" path="device/samsung/gts4lv" remote="github" />
  <project name="LineageOS/android_device_samsung_gts4lv-common" path="device/samsung/gts4lv-common" remote="github" />
  <project name="LineageOS/android_device_samsung_qcom-common" path="device/samsung/qcom-common" remote="github" />
  <project name="LineageOS/android_kernel_samsung_sdm670" path="kernel/samsung/sdm670" remote="github" />
  <project name="LineageOS/android_hardware_samsung" path="hardware/samsung" remote="github" />

  <project name="TheMuppets/proprietary_vendor_samsung" path="vendor/samsung" remote="github" />

  <remove-project name="LineageOS/android_device_samsung_gts4lv" />
  <project name="tom-pratt/android_device_samsung_gts4lv" path="device/samsung/gts4lv" remote="github" revision="main" />

  <remove-project name="LineageOS/android_device_samsung_gts4lv-common" />
  <project name="tom-pratt/android_device_samsung_gts4lv-common" path="device/samsung/gts4lv-common" remote="github" revision="main" />

  <remove-project name="LineageOS/android_kernel_samsung_sdm670" />
  <project name="tom-pratt/android_kernel_samsung_sdm670" path="kernel/samsung/sdm670" remote="github" revision="main" />
</manifest>
```