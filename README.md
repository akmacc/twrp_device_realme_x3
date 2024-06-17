TWRP Device configuration for realme x3 / superzoom (x3)

## Features

Works:
- Decryption of /data
- Screen brightness settings
- Correct screenshot color
- MTP
- Flashing (opengapps, roms, images and so on)
- Backup/Restore
- USB OTG

## Compile

First checkout minimal twrp source:

```
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
repo sync
git clone https://github.com/HyperTeam/twrp_device_realme_x3 -b twrp-12 device/realme/x3
```

Finally execute these:

```
. build/envsetup.sh
lunch twrp_x3-eng
mka recoveryimage
```
