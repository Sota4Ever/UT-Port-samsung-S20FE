# Requirements for installation

## Unlock bootloader
# ⚠️ Caution ⚠️
### Your device will have poor security, some Samsung functions will not work and it will be reset to factory settings blah blah blah :v
You already know the process for those who are experienced for that, for those who are new (like me) I will give you a guide:

1. Go to **Settings > About phone** and tap **Build number** 3 or more times to enable **Developer mode**.
2. Go back to **Settings**, open **Developer options**, and enable **OEM unlocking**. Enter your password if prompted.
3. Restart the device and quickly connect a **USB OTG** or USB cable to your computer.
4. While connecting, press **Volume Up + Volume Down** buttons simultaneously to enter **Odin mode**.
5. In Odin mode, press the volume up button to **unlock the bootloader**. The device will restart and reset to factory settings.

That's it! Your device will have the bootloader unlocked.

## Stock ROM (the original firmware)
For those who are using custom ROM, unfortunately you have to put STOCK ROM :(
You can find your firmware on the SM-G780F device page: [*samfw SM-G780F*](https://samfw.com/firmware/SM-G780F)

## Disable vbmeta
# ⚠️ Caution ⚠️
### It will be reset to factory settings
- Simple and easy just use your vbmeta and boot image of your firmware (Stock) which you probably still have downloaded
- Compress it in .tar format
- Use magisk to patch it will give you a new vbmeta image with the boot image
- There are two methods: on the computer [Odin3](https://samfw.com/Odin/Odin3_v3.13.1_3B_Patched_Samfw.com.rar) and with another device using [Heimdoo](https://github.com/RohitVerma882/Heimdoo/releases/download/v1.8/app-release.apk), to flash vbmeta image.
- Return your device to Odin mode, then press volume up

<details>
<summary><b><strong>Computer method💻(No images) </strong></b></summary>
  
- Connect your cable to your device; Odin3 should recognize the connected USB.
- In AB, place the compressed .tar file.
- Then click "Start", and your device will automatically reboot after that.
And that's it!

  </summary>
</details>

<details>
<summary><b><strong>Method on mobile📱(No images)</strong></b></summary>
You'll need to run commands to flash the vbmeta image in the application. Unzip the file and enter the following:
  
```
heimdall flash --VBMETA /path/to/vbmeta.img
```

Replace "/path/to/" with the actual folder location of your vbmeta.img file.


That's it!

  </summary>
</details>

## Use custom recovery image
To make the process easier [TWRP](https://t.me/s20femodding/1/164651) 
