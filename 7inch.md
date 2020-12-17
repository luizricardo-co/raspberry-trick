7inch screen enable

1. enter on /boot/config.txt

2. check disable_overscan is uncomment, by default is #disable_overscan=1
 - uncomment
disable_overscan=1

3. copy and paste commands bellow on bottom file

#7 inch HDMI LDC screen
max_usb_current=1
hdmi_force_hotplug=1
config_hdmi_boost=7
hdmi_group=2
hdmi_mode=87
hdmi_drive=1
hdmi_cvt 1020 600 60 6 0 0 0
gpu_mem=256
