# 7inch screen enable

Enter on config.txt

```sh
sudo nano /boot/config.txt
```

check if disable_overscan is comment, by default is #disable_overscan=1 and uncomment

```sh
disable_overscan=1
```

copy and paste commands bellow on end file

```sh
#7 inch HDMI LDC screen
max_usb_current=1
hdmi_force_hotplug=1
config_hdmi_boost=7
hdmi_group=2
hdmi_mode=87
hdmi_drive=1
hdmi_cvt 1020 600 60 6 0 0 0
gpu_mem=256
```

and the last

```sh
sudo reboot
```
