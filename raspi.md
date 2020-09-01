# Raspberr Pi Zero W

## DietPi
* So far best experience with [DietPi](https://dietpi.com]. Just flash it and follow the ncurses on-screen menu `dietpi-config`while selecting optimized software from the menus `dietpi-software`
* The [updated documentation](https://dietpi.com/docs/) looks nicer, though the BB system based information seems to be still accurate

# Raspberry Pi 3B

## DietPi
* Didn't check recently, but assumed to be similar as with the Zero W

## Open Suse

1. Even if there is a [common homepage](https://en.opensuse.org/HCL:Raspberry_Pi3) for Leap (stable) and Tumbleweed (rolling), the links are quickly outdated. Best way is to check on the [Tumbleweed General Download Directory](http://download.opensuse.org/ports/aarch64/tumbleweed/images/) or the [Leap General Download Directory](http://download.opensuse.org/ports/aarch64/distribution/leap/15.2/appliances/)
2. After flashing, at least Leap 15.2 will extend the filesystem to the whole SD card by itself
3. Bringing the system in a usable state:
  * Scale the display down to a usable size  `xrandr -s 1`
  
  * Activate the WiFi
  
       a) Remove `sdhci_iproc` from `/etc/dracut.conf.d/raspberrypi_modules.conf` and run `mkinitrd -f`
       
       b) Reboot
       
       c) Setup Wifi using *Yast Network* tool
   
  * Create a user utilizing *Yast Users and Groups*
  * Install nano :wink: `zypper in nano`

## *Ubuntu Server + FVWM Crystal*

### DE
Login Manager: `ly` (`tbsm`,`XDM` as alternatives)
Most information available in the [Gentoo Wiki](https://wiki.gentoo.org/wiki/FVWM-Crystal)
Current Minimal List:

>  sudo apt install xserver-xorg-core xinit menu menu-xdg gdebi-core logrotate localepurge

>  sudo apt install build-essential

>  wget https://sourceforge.net/projects/fvwm-crystal/files/3.6.6/fvwm-crystal-3.6.6.tar.gz

>  tar xzvf fvwm-crystal-3.6.6.tar.gz

>  cd fvwm-crystal-3.6.6/

>  sudo make prefix=/usr install

>  sudo apt install rox-filer pcmanfm fvwm xterm xscreensaver alsaplayer mplayer pmount

>  sudo groupadd fvwm-crystal

>  sudo usermod -aG dialout,cdrom,floppy,audio,video,plugdev,fvwm-crystal,fuse,lpadmin USERNAME

Create .xsession file and add `exec fvwm-crystal`


### OS
Currently planned is [Ubuntu Server 20.04 64bit](https://ubuntu.com/download/raspberry-pi) see on the [Ubuntu Minimal Desktop](http://wiki.dennyhalim.com/ubuntu-minimal-desktop) page what missing packages to install
