# Kiosk installer for Debian based Linux distros
Small installer script to setup a minimal kiosk with Chromium for Debian based Linux distros. This installer is heavily based on the excellent [instructions by Will Haley](http://willhaley.com/blog/debian-fullscreen-gui-kiosk/).

## Usage
* Setup a minimal Debian without display manager, e.g. Armbian
* Login as root or with root permissions
* Download this installer, make it executable and run it

  ```shell
  wget https://github.com/clubshrimp/debian-kiosk-installer/blob/master/kiosk-installer.sh; chmod +x kiosk-installer.sh; ./kiosk-installer.sh
  ```

## What will it do?
It will create a normal user `kiosk`, install software (check the script) and setup configs (it will backup existing) so that on reboot the kiosk user will login automaticaly and run chromium in kiosk mode with one url. It will also hide the mouse. 

## Change the url
Change the url at the bottom of the script, where it sais https://neave.tv/

## Is it secure?
No. Although it will run as a normal user (and I suggest you don't leave a keyboard and mouse hanging around), there will be the possibility of plugin' in a mini keyboard, opening a terminal and opening some nasty things. Security is your thing ;-) 
