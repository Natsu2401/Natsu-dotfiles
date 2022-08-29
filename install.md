/etc/X11/xorg.conf.d/100-touchpad.conf

Section "InputClass"
        Identifier "libinput touchpad catchall"
        MatchIsTouchpad "on"
        MatchDevicePath "/dev/input/event*"
        Driver "libinput"
    Option "Tapping" "on"
    Option "NaturalScrolling" "true"
    Option "ClickMethod" "clickfinger"
    Option "TappingButtonMap" "lrm"
    Option "DisableWhileTyping" "true"
EndSection