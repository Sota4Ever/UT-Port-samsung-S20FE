# Installation

*For installation you have to review [Requirements for installation](https://github.com/Sota4Ever/samsung-S20FE/blob/halium-13-r8s/Requirements-for-installation.md)*

### Put the device in Odin mode (Download)
It is similar to disabling vbmeta in exchange for only replacing the recovery image, but in device method you only have to change

```
heimdall flash --RECOVERY /path/to/recovery.img
```

Replace "/path/to/" with the actual folder location of your recovery.img file.

### Put the device in recovery mode
Press VOLUMEN UP + POWER BUTTON with the cable connected to a device

- ### Format the following partitions
<div style="display: flex; justify-content: flex-start; align-items: center;">
    <img src="Screenshots/Screenshot_2024-09-26-19-32-46.png" width="200" alt="Screenshot 1" style="margin-right: 10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-32-50.png" width="200" alt="Screenshot 2" style="margin-right: 10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-35-47.png" width="200" alt="Screenshot 3" style="margin-right: 10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-37-42.png" width="200" alt="Screenshot 4">
</div>

- ### Flash the boot image (boot.img)
<div style="display: flex; justify-content: flex-start; align-items: center; margin-bottom: 10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-35-47.png" width="200" alt="Screenshot 1" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-31-20.png" width="200" alt="Screenshot 2" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-31-24.png" width="200" alt="Screenshot 3" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-31-41.png" width="200" alt="Screenshot 4">
</div>

### Put ext4 format on the /data partition
<div style="display: flex; justify-content: flex-start; align-items: center; margin-bottom: 10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-35-47.png" width="200" alt="Screenshot 1" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-19-32-46.png" width="200" alt="Screenshot 2" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-55-16.png" width="200" alt="Screenshot 3" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-49-50.png" width="200" alt="Screenshot 4" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-49-50.png" width="200" alt="Screenshot 5" style="margin-right:10px;">
    <img src="Screenshots/Screenshot_2024-09-26-20-50-04.png" width="200" alt="Screenshot 6">
</div>

*Swipe to change*

### Copy the ubuntu.img image to the /data partition

Lots of images, I'll just say quickly.

- At the beginning go to `Advanced` and in options there it says `Terminal`
 - Copy the ubuntu.img image to the /data partition
 ```
 cp -r ubuntu.img /data
 ```
 When you finish copying the image, it's done.

______________________
 # You finished and now restart the device and enjoy Ubuntu Touch :D
