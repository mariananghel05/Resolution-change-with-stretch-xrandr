# Resolution-change-with-stretch-xrandr
xrandr --output eDP-1-1 --mode 1920x1080 --set "scaling mode" "Full"


script for dmenu


#!/bin/bash
 dinput () {
            (echo -e "1920x1080\n1280x1024"   | dmenu -i -p "Resolution:") <&-
            }

            url=$(dinput)
            xrandr --output eDP-1-1 --mode $url --set "scaling mode" "Full"
