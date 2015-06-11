openwrt-xiaomi-mini
==============

OpenWrt Patch for Xiaomi Router Mini

#### How to compile the firmware:

    git clone https://github.com/rssnsj/openwrt-xiaomi-mini.git
    cd openwrt-xiaomi-mini
    make

#### Flashing the firmware generated above:

* Before you flash the new firmware for the first time, visit（ https://d.miwifi.com/rom/ssh ），and bind the device to your MiWiFi account. Then log in to it and run the command below to load the new SSH-enabled binary：

    `mtd -r write openwrt-ramips-mt7620a-xiaomi-miwifi-mini-squashfs-sysupgrade.bin firmware`

* Then flash this to upgrade after running the command above：

    `sysupgrade openwrt-ramips-mt7620a-xiaomi-miwifi-mini-squashfs-sysupgrade.bin`
