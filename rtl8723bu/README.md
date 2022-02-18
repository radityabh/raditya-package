Add Driver wifi rtl8723bu ds866 to Openwrt

Clone this folder to /package/kernel

add in .config `CONFIG_PACKAGE_kmod-rtl8723bu=y`

if wifi still not work please run this command & reboot

```
sed -i "s|iw |ipconfig |g"  /lib/netifd/wireless/mac80211.sh
```