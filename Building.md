# Building

## Recommendation

*I recommend distribution: Ubuntu 22.04.3 LTS*
*or you can also use [GitHub codespace](https://github.com/features/codespaces)*

First of all you have to install the packages needed for the build, for the ones you have it is not necessary

```
sudo apt-get update -y && sudo apt-get install dialog bash sed wget git curl zip tar jq expect make cmake automake autoconf llvm lld lldb clang gcc binutils bison perl gperf gawk flex bc python3 python2 zstd openssl unzip cpio bc bison build-essential ccache liblz4-tool libsdl1.2-dev libstdc++6 libxml2 libxml2-utils lzop pngcrush schedtool squashfs-tools xsltproc zlib1g-dev libncurses5-dev bzip2 git gcc g++ libssl-dev gcc-aarch64-linux-gnu gcc-arm-linux-gnueabihf gcc-arm-linux-gnueabi libtinfo5 dwarves libelf-dev resolvconf dos2unix python3 python2 python-is-python3 kmod neofetch img2simg fakeroot -y
```
----------------------

### Step 1
Clone the repository:
```
git clone https://github.com/Sota4Ever/UT-Port-samsung-S20FE.git -b halium-13-r8s --depth 1
```

### Step 2
Build and wait for it to finish with the following command:
```
./build.sh -b workdir
```

### Step 3
Once completed, run the next command:
```
./build/prepare-fake-ota.sh out/device_r8s_usrmerge.tar.xz ota
```

This will download files, extract, and compress.

### Step 4
Now, prepare images with the following command:
```
./build/system-image-from-ota.sh ota/ubuntu_command images
```

The following files will appear in the "images" folder:

 - system.img (not necessary)
 - rootfs.img            
 - boot.img

Rename the `rootfs.img` image to `ubuntu.img`.
