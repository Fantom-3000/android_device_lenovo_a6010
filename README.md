Unified Device Tree for Lenovo a6010 based on Moto G 2015 (osprey)
===========================================



Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Quad-core 1.4 GHz Cortex-A53
Chipset | Qualcomm MSM8916 Snapdragon 410
GPU     | Adreno 306
Memory  | 1/2 GB RAM
Shipped Android Version | 5.1.1
Storage | 8/16 GB
MicroSD | Up to 32 GB
Battery | Li-Ion 2470mAh battery
Display | 720 x 1280 pixels, 5.0 inches (~294 ppi pixel density)
Camera  | 13 MP, 4160 x 2340 pixels, autofocus, dual flash LED





# How To Compile

Please note it is based on Motorola Osprey source. you need to replace lenovo a6010 files. make sure you changed everything.

I am givining you idea only. i can not say it will work. but it should work. play with this. change what you need and what you have.

You need following

#1. device tree for lenovo a6010 

https://github.com/jsharma44/android_device_lenovo_a6010


path:  device/lenovo/a6010

#2. common  device tree msm8916
https://github.com/jsharma44/android_device_lenovo_msm8916-common

path:  device/lenovo/msm8916-common

#3. vendor tree for lenovo a6010

this is based on motoroloa osprey so extract files from your device and change here.

https://github.com/jsharma44/android_vendor_lenovo_a6010

Path: vendor/lenovo/a6010


#4. vender tree for common msm8916

this is based on motoroloa osprey so extract files from your device and change here.

https://github.com/jsharma44/android_vendor_lenovo_common_msm8916

Path: vendor/lenovo/msm8916-common

#5.  Kernel for lenovo a6010

this is 3.10 kernel

https://github.com/jsharma44/android_kernel_lenovo_a6010

Path: kernel/lenovo/a6010

#6.  Other cm.dependencies

These are CynogenMod dependenciec. serach for them in https://github.com/CyanogenMod  download them and copy them to your source code/path

[
 
  {
    "repository": "android_external_bson",
    "target_path": "external/bson"
  },
  {
    "repository": "android_device_qcom_common",
    "target_path": "device/qcom/common"
  },
  {
    "repository": "android_packages_resources_devicesettings",
    "target_path": "packages/resources/devicesettings"
  }
]



Make sure you replaced your device files. you can extract binary blobs from your device.  do it and put them in right folder.


To compile it

a. source build/envsetup.sh
b. lunch

select device a6010

c. make 







# Work in Progress.    I hope you can do it for lenovo a6010 .  I dont have this device. I did this for a user who requested.



 






