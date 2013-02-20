rt5370sta
=========

RT5370 Driver ready for work on Debian Squeeze.

I changed two lines in 'os/linux/config.mk' that make wpa_supplicant work for this driver.

In line 57, 'HAS_WPA_SUPPLICANT=n' to 'HAS_WPA_SUPPLICANT=y'
and in line 61, 'HAS_NATIVE_WPA_SUPPLICANT_SUPPORT=n' to  'HAS_NATIVE_WPA_SUPPLICANT_SUPPORT=y'

To install do:

sudo make clean
sudo make
sudo make install

To use do:

sudo modprobe rt5370sta