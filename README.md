# libinput_quirks
Quirks file for libinput under Wayland on a MacBook Pro (7,1) Mid-2010. I've tested this under Kali, Fedora 30 and Ubuntu 19.04. 

Based on this article: https://wayland.freedesktop.org/libinput/doc/latest/touchpad-pressure-debugging.html

I was able to come up with a quirks file that made my trackpad work much better.

The linked article shows the trackpad as /dev/input/event10. Mine is /dev/input/event9, yours may vary. It's a bit of trial and error using the **libinput --measure** command and testing your pressure settings. It also will vary depending on the size of your fingers and your preferred style of mousing. You'll likely need to install libinput-tools using **apt**, **dnf** or whatever your distribution needs before you can test your trackpad.

Here's all the available quirks for libinput. https://wayland.freedesktop.org/libinput/doc/latest/device-quirks.html
