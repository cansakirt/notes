# notes

## Raspberry Pi NOOBS installation:

1. Format SD card
2. Extract noobs.zip into sd card
3. Put wpa_supplicant.conf in NOOBS root dir
  add this after mount inside /os/Raspbian/partition_setup.sh       
  `if [ -e /settings/wpa_supplicant.conf ] ; then cp /settings/wpa_supplicant.conf /tmp/2/etc/wpa_supplicant/wpa_supplicant.conf ; fi`
4. Enable vnc
  add `vncinstall` to the end of /recovery.cmdline
5. should work.
