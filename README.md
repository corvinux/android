For Sony Xperia Tablet Z - pollux, pollux_windy

Latest version, not working

- To get the required device repositories, add the local_manifest.xml file to .repo/local_manifests and do a repo sync
- Following the Porting Guide, update the kernel config with the check-config script
- You can use these commits:
  - https://github.com/mamenyaka/android_device_sony_pollux-common/commit/9c1b00c106f4ab3e66845cc98a726c1edef98b15
  - https://github.com/mamenyaka/android_device_sony_fusion3-common/commit/221cab6c6f43a40343fc4db0e5e90e04550dda1f
  - https://github.com/mamenyaka/android_kernel_sony_apq8064/commit/3d8086344907977512d0c6ed838711dcb2b7eee2
  - https://github.com/mamenyaka/android_kernel_sony_apq8064/commit/7e405137202496fbfa6dc9d6ceedeec24aa1949a
- Apply the changes in main.patch to build/core/main.mk
- Apply the changes in rootstock.path to project-rootstock-ng/rootstock-touch-install
- Build and install
